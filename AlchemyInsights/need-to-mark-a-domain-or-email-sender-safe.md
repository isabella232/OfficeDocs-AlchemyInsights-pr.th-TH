---
title: ต้องการทำเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803264"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1967f-102">ต้องการทำเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่</span><span class="sxs-lookup"><span data-stu-id="1967f-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1967f-103">**ไม่แนะนำให้ใช้รายชื่อผู้ส่งที่ปลอดภัย**เนื่องจากจะเปิดองค์กรของคุณให้เป็นสแปม, phish และการโจมตีของการปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="1967f-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1967f-104">อย่างไรก็ตามถ้ามีความต้องการทางธุรกิจเรา **ขอแนะนำ** ให้ใช้ **[กฎการไหลของจดหมาย](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** สำหรับการดำเนินการนี้</span><span class="sxs-lookup"><span data-stu-id="1967f-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1967f-105">คำแนะนำของเราช่วยให้แน่ใจว่าผู้ส่งรับรองความถูกต้อง (ตรวจสอบโดเมนที่ส่งไม่ถูกปลอม)</span><span class="sxs-lookup"><span data-stu-id="1967f-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1967f-106">**หมายเหตุ**: เราไม่แนะนำให้จัดการการบวก false โดยใช้รายชื่อผู้ส่งที่ปลอดภัยเนื่องจากมีข้อยกเว้นในการกรองสแปมสามารถเปิดองค์กรของคุณเพื่อการโจมตีด้านความปลอดภัยได้</span><span class="sxs-lookup"><span data-stu-id="1967f-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1967f-107">ถ้าผู้ใช้ของคุณได้รับข้อความที่ถูกทำเครื่องหมายเป็นสแปมหรืออีเมลขยะอย่างไม่ถูกต้องโปรด**[รายงานข้อความและไฟล์ไปยังไมโครซอฟท์](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="1967f-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1967f-108">ผู้ส่งที่ปลอดภัยใน Outlook, รายชื่อผู้ส่งที่ได้รับอนุญาตหรือรายการโดเมนที่อนุญาตในนโยบายการป้องกันสแปม **ควรหลีกเลี่ยง** เนื่องจากผู้ส่งเลี่ยงผ่านสแปม, หลอกลวงและ phish และการรับรองความถูกต้องของผู้ส่ง (SPF, DKIM, DMARC)</span><span class="sxs-lookup"><span data-stu-id="1967f-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1967f-109">วิธีนี้ใช้ได้ดีที่สุดสำหรับการทดสอบชั่วคราวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="1967f-109">This method is best used for temporary testing only.</span></span>
