---
title: ต้องการทําเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281190"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="83947-102">ต้องการทําเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่</span><span class="sxs-lookup"><span data-stu-id="83947-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="83947-103">**ไม่แนะนําให้ใช้รายชื่อผู้ส่งที่ปลอดภัย**เนื่องจากเปิดองค์กรของคุณเป็นสแปม ฟิช และการปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="83947-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="83947-104">อย่างไรก็ตาม หากมีความต้องการทางธุรกิจ**เราขอแนะนําให้ใช้\*\*\*\*[กฎขั้นตอนจดหมาย](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** สําหรับสิ่งนี้</span><span class="sxs-lookup"><span data-stu-id="83947-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="83947-105">คําแนะนําของเราทําให้การตรวจสอบสิทธิ์ผู้ส่ง (ตรวจสอบความถูกต้องของผู้ส่งไม่ได้ถูกปลอมแปลง)</span><span class="sxs-lookup"><span data-stu-id="83947-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="83947-106">**หมายเหตุ**: เราไม่แนะนําให้จัดการค่าบวกที่ผิดพลาดโดยใช้รายชื่อผู้ส่งที่ปลอดภัย เนื่องจากข้อยกเว้นในการกรองสแปมสามารถเปิดองค์กรของคุณเพื่อการโจมตีด้านความปลอดภัยได้</span><span class="sxs-lookup"><span data-stu-id="83947-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="83947-107">ถ้าผู้ใช้ของคุณได้รับข้อความที่ถูกทําเครื่องหมายว่าเป็นอีเมลขยะหรืออีเมลขยะอย่างไม่ถูกต้อง**[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="83947-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="83947-108">ผู้ส่งที่ปลอดภัยใน Outlook รายชื่อผู้ส่งที่ได้รับอนุญาต หรือรายการที่อนุญาตในนโยบายป้องกันสแปม**ควรหลีกเลี่ยง**เนื่องจากผู้ส่งจะข้ามสแปม การปลอมแปลง และการป้องกันฟิชเชอร์ทั้งหมด และการตรวจสอบสิทธิ์ของผู้ส่ง (SPF, DKIM, DMARC)</span><span class="sxs-lookup"><span data-stu-id="83947-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="83947-109">วิธีนี้จะใช้ได้ดีที่สุดสําหรับการทดสอบชั่วคราวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="83947-109">This method is best used for temporary testing only.</span></span>
