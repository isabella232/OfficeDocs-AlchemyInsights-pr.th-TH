---
title: ขั้นตอนที่แนะนําในการพิจารณาหากบัญชีถูกบุกรุก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: a094862a175184c3ac2a717cc59aefe2470b9fd1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510807"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="7af77-102">ขั้นตอนที่แนะนําในการพิจารณาหากบัญชีถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="7af77-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="7af77-103">วิดีโอ: การแก้ไขบัญชีที่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="7af77-103">VIDEO: Fixing a compromised account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="7af77-104">[รีเซ็ตรหัสผ่านของผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords)ทันที</span><span class="sxs-lookup"><span data-stu-id="7af77-104">[Reset the user's password](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="7af77-105">อย่าสื่อสารรหัสผ่านใหม่ผ่านทางอีเมลไปยังผู้ใช้ปลายทาง</span><span class="sxs-lookup"><span data-stu-id="7af77-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="7af77-106">เอา[ที่อยู่การส่งต่อ](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)ที่น่าสงสัยใด ๆ ที่ตั้งค่าไว้ที่ระดับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="7af77-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="7af77-107">ลบ[กฎกล่องจดหมาย](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED)ที่น่าสงสัยใด ๆ ที่ตั้งค่าภายในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="7af77-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="7af77-108">ถ้าผู้ใช้ถูกบล็อกไม่ให้ส่งอีเมล[ให้ไปที่หน้าผู้ใช้ที่จํากัดเพื่อยกเลิกการบล็อกบัญชี](https://protection.office.com/?hash=/restrictedusers)</span><span class="sxs-lookup"><span data-stu-id="7af77-108">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="7af77-109">เมื่อทําเสร็จแล้วผู้ใช้ควรจะสามารถส่งข้อความต่อภายใน 1 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="7af77-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="7af77-110">เอาบัญชีผู้ใช้ออกจาก[กลุ่มบทบาทผู้ดูแล](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles)ใดๆ จนกว่าคุณมั่นใจว่าบัญชีจะไม่ถูกบุกรุกอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="7af77-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="7af77-111">เราแนะนําให้อ่าน[แผนงานด้านความปลอดภัย Microsoft 365](https://docs.microsoft.com//office365/securitycompliance/security-roadmap)ของเราเพื่อลดโอกาสของการละเมิดข้อมูลหรือบัญชีที่ถูกบุกรุกในอนาคต</span><span class="sxs-lookup"><span data-stu-id="7af77-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Microsoft 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  