---
title: ขั้นตอนที่แนะนำในการดำเนินการหากบัญชีถูกบุกรุก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 08904708dd19104179c3f97f6734d8af725a4512
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745452"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="2d88b-102">ขั้นตอนที่แนะนำในการดำเนินการหากบัญชีถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="2d88b-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="2d88b-103">วิดีโอ: แก้ไขบัญชี Office ๓๖๕ที่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="2d88b-103">VIDEO: Fixing a compromised Office 365 account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="2d88b-104">[รีเซ็ตรหัสผ่านของผู้ใช้](https://docs.microsoft.com/office365/admin/add-users/reset-passwords)ทันที</span><span class="sxs-lookup"><span data-stu-id="2d88b-104">[Reset the user's password](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="2d88b-105">อย่าสื่อสารรหัสผ่านใหม่ผ่านทาง e-mail ไปยังผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="2d88b-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="2d88b-106">ลบที่[อยู่การส่งต่อ](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding)ที่น่าสงสัยที่ตั้งอยู่ในระดับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="2d88b-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="2d88b-107">เอากฎของ[กล่องขาเข้า](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED)ที่น่าสงสัยใดๆที่ตั้งอยู่ภายในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="2d88b-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="2d88b-108">หากผู้ใช้ถูกบล็อกไม่ให้ส่งทาง e-mail[ไปที่หน้าผู้ใช้ที่ถูกจำกัดเพื่อยกเลิกการบล็อคบัญชี](https://protection.office.com/?hash=/restrictedusers)</span><span class="sxs-lookup"><span data-stu-id="2d88b-108">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="2d88b-109">เมื่อเสร็จแล้วผู้ใช้ควรจะสามารถที่จะดำเนินการส่งข้อความภายใน1ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="2d88b-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="2d88b-110">เอาบัญชีผู้ใช้ออกจาก[กลุ่มบทบาทการดูแลระบบ](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles)ใดๆจนกว่าคุณจะมั่นใจว่าบัญชีจะไม่ถูกบุกรุกอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="2d88b-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="2d88b-111">เพื่อลดศักยภาพของการละเมิดข้อมูลหรือบัญชีที่ถูกบุกรุกในอนาคตเราขอแนะนำให้อ่าน[แผนการรักษาความปลอดภัย Office ๓๖๕](https://docs.microsoft.com//office365/securitycompliance/security-roadmap)ของเรา</span><span class="sxs-lookup"><span data-stu-id="2d88b-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Office 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  