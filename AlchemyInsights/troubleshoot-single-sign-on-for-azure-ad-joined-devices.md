---
title: แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037335"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="b0823-102">แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD</span><span class="sxs-lookup"><span data-stu-id="b0823-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="b0823-103">ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD กับ Azure AD คุณสามารถทํางานนี้ได้โดยการเข้าร่วม Azure AD แบบไฮบริด</span><span class="sxs-lookup"><span data-stu-id="b0823-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="b0823-104">[วิธีการ: วางแผนการปรับใช้การเข้าร่วม Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) แบบไฮบริดจะให้คุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="b0823-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="b0823-105">ดูข้อมูลเพิ่มเติมในการกําหนด [ค่าอุปกรณ์ที่เข้าร่วมของ Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)Single-Signเปิดใช้งาน Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="b0823-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="b0823-106">**ปัญหาโทเค็นรีเฟรชหลัก (PRT)**</span><span class="sxs-lookup"><span data-stu-id="b0823-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="b0823-107">โทเค็นรีเฟรชหลัก (PRT) คือสิ่งประดิษฐ์หลักของการรับรองความถูกต้อง Azure AD บนอุปกรณ์ Windows 10, Windows Server 2016 และเวอร์ชันที่ใหม่กว่า, iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="b0823-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="b0823-108">ซึ่งเป็นโทเค็นเว็บ JSON (JWT) ที่ออกให้กับนายหน้าโทเค็นของบริษัทแรกใน Microsoft เพื่อเปิดใช้งานการลงชื่อเข้าระบบครั้งเดียว (SSO) ในแอปพลิเคชันที่ใช้บนอุปกรณ์เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="b0823-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="b0823-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="b0823-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="b0823-110">**WamDefaultSet: YES และ AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="b0823-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="b0823-111">เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้องไปยัง Azure AD เรียบร้อยแล้วหรือไม่เมื่อลงชื่อเข้าใช้อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="b0823-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="b0823-112">ถ้าค่าเป็น **NO** อาจเป็นเพราะ:</span><span class="sxs-lookup"><span data-stu-id="b0823-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="b0823-113">คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)</span><span class="sxs-lookup"><span data-stu-id="b0823-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="b0823-114">รหัสการเข้าสู่ระบบอื่น</span><span class="sxs-lookup"><span data-stu-id="b0823-114">Alternate Login ID</span></span>
- <span data-ttu-id="b0823-115">ไม่พบพร็อกซี HTTP</span><span class="sxs-lookup"><span data-stu-id="b0823-115">HTTP Proxy not found</span></span>

<span data-ttu-id="b0823-116">เมื่อต้องการแก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd ให้ดู[สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="b0823-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
