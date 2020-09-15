---
title: ๖๔๖วิธีการกำหนดค่า AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704508"
---
# <a name="configure-sync-features"></a><span data-ttu-id="0e240-102">กำหนดค่าฟีเจอร์การซิงค์</span><span class="sxs-lookup"><span data-stu-id="0e240-102">Configure sync features</span></span>

<span data-ttu-id="0e240-103">Azure AD Connect มีฟีเจอร์หลายอย่างที่จะเปิดใช้งานตามค่าเริ่มต้นหรือคุณสามารถเปิดใช้งานในภายหลังได้</span><span class="sxs-lookup"><span data-stu-id="0e240-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="0e240-104">ฟีเจอร์บางอย่างจำเป็นต้องมีการกำหนดค่าเพิ่มเติมในสภาพแวดล้อมที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="0e240-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="0e240-105">การ[กรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)จำกัดวัตถุจะถูกซิงโครไนซ์กับ Azure AD</span><span class="sxs-lookup"><span data-stu-id="0e240-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="0e240-106">ตามค่าเริ่มต้นผู้ใช้ที่ติดต่อกลุ่มและบัญชีผู้ใช้ Windows 10 ทั้งหมดจะถูกซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="0e240-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="0e240-107">คุณสามารถรวมหรือแยกวัตถุได้โดยยึดตามโดเมน Ou หรือแอตทริบิวต์อื่นๆ</span><span class="sxs-lookup"><span data-stu-id="0e240-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="0e240-108">การ[ซิงโครไนซ์แฮชของรหัสผ่านซิ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)งโครไนซ์แฮชของรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรไปยัง Azure AD</span><span class="sxs-lookup"><span data-stu-id="0e240-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="0e240-109">การทำเช่นนี้จะช่วยให้การจัดการรหัสผ่านในตำแหน่งที่ตั้งเดียวแต่ใช้รหัสผ่านเดียวกันในสภาพแวดล้อมทั้งภายในองค์กรและระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="0e240-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="0e240-110">เนื่องจาก Active Directory เป็นแหล่งข้อมูลที่มีสิทธิ์คุณสามารถใช้นโยบายรหัสผ่านของคุณเองได้</span><span class="sxs-lookup"><span data-stu-id="0e240-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="0e240-111">การ[ตั้งค่ารหัสผ่านแบบบริการตนเอง (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)อนุญาตให้ผู้ใช้รีเซ็ตรหัสผ่านของตนเองในระบบคลาวด์ได้ในขณะที่ยังคงใช้นโยบายรหัสผ่านภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="0e240-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="0e240-112">[อุปกรณ์ writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ช่วยให้อุปกรณ์ที่ลงทะเบียนใน Azure AD จะถูกเขียนกลับไปยัง active directory ภายในองค์กรเพื่อให้สามารถใช้สำหรับการเข้าถึงแบบมีเงื่อนไขได้</span><span class="sxs-lookup"><span data-stu-id="0e240-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="0e240-113">การ[ป้องกันการลบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)โดยไม่ตั้งใจจะถูกเปิดใช้งานตามค่าเริ่มต้นเพื่อช่วยป้องกันไม่ให้มีการลบวัตถุพร้อมกันจำนวนมากเกินไป (วัตถุมากกว่า๕๐๐ต่อการซิงโครไนซ์)</span><span class="sxs-lookup"><span data-stu-id="0e240-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="0e240-114">คุณสามารถเปลี่ยนการตั้งค่านี้เพื่อตอบสนองความต้องการขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="0e240-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="0e240-115">การ[อัปเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)จะถูกเปิดใช้งานตามค่าเริ่มต้นสำหรับการติดตั้งแบบด่วนและช่วยให้แน่ใจว่าเวอร์ชันของ Azure AD Connect ของคุณเป็นปัจจุบันเสมอ</span><span class="sxs-lookup"><span data-stu-id="0e240-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
