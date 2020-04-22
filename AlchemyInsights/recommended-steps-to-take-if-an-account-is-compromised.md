---
title: ขั้นตอนที่แนะนําสําหรับกรณีที่บัญชีถูกบุกรุก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 616107f1a5297b38637118e93ee6bfb918640ab3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719323"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="cf8ca-102">ขั้นตอนที่แนะนําสําหรับกรณีที่บัญชีถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="cf8ca-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="cf8ca-103">วิดีโอ: การแก้ไขบัญชีที่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="cf8ca-103">VIDEO: Fixing a compromised account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="cf8ca-104">[รีเซ็ตรหัสผ่านของผู้ใช้](https://docs.microsoft.com/office365/admin/add-users/reset-passwords)ทันที</span><span class="sxs-lookup"><span data-stu-id="cf8ca-104">[Reset the user's password](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="cf8ca-105">อย่าสื่อสารรหัสผ่านใหม่ผ่านทางอีเมลไปยังผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="cf8ca-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="cf8ca-106">ลบ[ที่อยู่การส่งต่อ](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding)ที่น่าสงสัยใดๆ ที่ตั้งค่าไว้ที่ระดับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="cf8ca-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="cf8ca-107">เอา[กฎกล่องจดหมาย](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED)ที่น่าสงสัยใดๆ ที่ตั้งค่าไว้ในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="cf8ca-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="cf8ca-108">หากผู้ใช้ถูกบล็อกไม่ให้ส่งอีเมล[ให้ไปที่หน้า ผู้ใช้ที่ถูกจํากัด เพื่อยกเลิกการบล็อกบัญชีผู้ใช้](https://protection.office.com/?hash=/restrictedusers)</span><span class="sxs-lookup"><span data-stu-id="cf8ca-108">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="cf8ca-109">เมื่อเสร็จแล้วผู้ใช้ควรจะสามารถกลับมาส่งข้อความภายใน 1 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="cf8ca-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="cf8ca-110">เอาบัญชีผู้ใช้ออกจาก[กลุ่มบทบาทผู้ดูแล](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles)ใด ๆ จนกว่าคุณมั่นใจว่า บัญชีจะไม่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="cf8ca-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="cf8ca-111">เราขอแนะนําให้อ่าน[แผนงานด้านความปลอดภัยของ Microsoft 365 ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap)</span><span class="sxs-lookup"><span data-stu-id="cf8ca-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Microsoft 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  