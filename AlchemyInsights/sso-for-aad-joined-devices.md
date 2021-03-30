---
title: Single-Signเปิดบนอุปกรณ์ที่เข้าร่วมของ Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405663"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="30412-102">การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="30412-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="30412-103">ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD กับ Azure AD คุณสามารถทํางานนี้ให้เสร็จได้โดยการเข้าร่วม Azure AD แบบไฮบริด</span><span class="sxs-lookup"><span data-stu-id="30412-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="30412-104">[วิธีการ: วางแผนการปรับใช้การเข้าร่วม Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) แบบไฮบริดจะให้คุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="30412-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="30412-105">กําหนดค่าอุปกรณ์ที่เข้าร่วมของ Azure AD Single-Signภายในองค์กรโดยใช้ Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="30412-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="30412-106">**ปัญหาโทเค็นรีเฟรชหลัก (PRT)** โทเค็นรีเฟรชหลัก (PRT) คือสิ่งประดิษฐ์หลักของการรับรองความถูกต้อง Azure AD บน Windows 10, Windows Server 2016 และเวอร์ชันที่ใหม่กว่า, iOS และอุปกรณ์ Android</span><span class="sxs-lookup"><span data-stu-id="30412-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="30412-107">ซึ่งเป็นโทเค็นเว็บ JSON (JWT) ที่ออกให้กับนายหน้าโทเค็นของบริษัทแรกใน Microsoft เพื่อเปิดใช้งานการลงชื่อเข้าระบบครั้งเดียว (SSO) ในแอปพลิเคชันที่ใช้บนอุปกรณ์เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="30412-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="30412-108">[โทเค็นรีเฟรชหลักคืออะไร เราจะ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)ให้รายละเอียดเกี่ยวกับวิธีการออก ใช้ และป้องกัน PRT บนอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="30412-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="30412-109">**WamDefaultSet: YES และ AzureADPrt: YES** เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้องไปยัง Azure AD เรียบร้อยแล้วหรือไม่เมื่อลงชื่อเข้าใช้อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="30412-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="30412-110">ถ้าค่าเป็น **NO** อาจเป็นเพราะ:</span><span class="sxs-lookup"><span data-stu-id="30412-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="30412-111">คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)</span><span class="sxs-lookup"><span data-stu-id="30412-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="30412-112">รหัสการเข้าสู่ระบบอื่น</span><span class="sxs-lookup"><span data-stu-id="30412-112">Alternate Login ID</span></span>
- <span data-ttu-id="30412-113">ไม่พบพร็อกซี HTTP</span><span class="sxs-lookup"><span data-stu-id="30412-113">HTTP Proxy not found</span></span>

<span data-ttu-id="30412-114">แก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd - [สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="30412-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
