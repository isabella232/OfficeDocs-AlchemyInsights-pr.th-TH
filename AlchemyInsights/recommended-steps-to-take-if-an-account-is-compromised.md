---
title: ขั้นตอนที่แนะนำในการดำเนินการถ้าบัญชีผู้ใช้ถูกบุกรุก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: acce676ebb9f4000794669ffb268e7b4fe057f77
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771299"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="55f88-102">ขั้นตอนที่แนะนำในการดำเนินการถ้าบัญชีผู้ใช้ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="55f88-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="55f88-103">วิดีโอ: การแก้ไขบัญชีผู้ใช้ที่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="55f88-103">VIDEO: Fixing a compromised account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="55f88-104">[ตั้งค่ารหัสผ่านของผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) ทันที</span><span class="sxs-lookup"><span data-stu-id="55f88-104">[Reset the user's password](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="55f88-105">อย่าสื่อสารรหัสผ่านใหม่ผ่านทางอีเมลไปยังผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="55f88-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="55f88-106">เอา [ที่อยู่การส่งต่อ](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) ที่น่าสงสัยที่ตั้งค่าไว้ที่ระดับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="55f88-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="55f88-107">เอา [กฎกล่องจดหมายเข้า](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) ที่น่าสงสัยไว้ภายในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="55f88-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="55f88-108">ถ้าผู้ใช้ถูกบล็อกจากการส่งอีเมลให้ [ไปที่หน้าผู้ใช้ที่ถูกจำกัดเพื่อยกเลิกการบล็อกบัญชีผู้](https://protection.office.com/?hash=/restrictedusers)ใช้</span><span class="sxs-lookup"><span data-stu-id="55f88-108">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="55f88-109">เมื่อเสร็จแล้วผู้ใช้ควรจะสามารถส่งข้อความภายใน1ชั่วโมงต่อไปได้</span><span class="sxs-lookup"><span data-stu-id="55f88-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="55f88-110">เอาบัญชีผู้ใช้ออกจาก [กลุ่มบทบาทการดูแลระบบ](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) ใดๆจนกว่าคุณจะมั่นใจว่าบัญชีผู้ใช้นั้นจะไม่ถูกบุกรุกอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="55f88-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="55f88-111">เมื่อต้องการลดศักยภาพของการละเมิดข้อมูลหรือบัญชีผู้ใช้ที่ถูกบุกรุกในอนาคตเราขอแนะนำให้อ่าน [แผนการรักษาความปลอดภัย Microsoft ๓๖๕ ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap)ของเรา</span><span class="sxs-lookup"><span data-stu-id="55f88-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Microsoft 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  