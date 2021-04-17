---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821466"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="01d4f-102">แก้ไขปัญหาการส่งรหัสข้อผิดพลาด 550 5.4.1 การเข้าถึงรีเลย์ถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="01d4f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="01d4f-103">ปัญหานี้เกิดขึ้นเมื่อ [ตรวจสอบเพื่อดูว่าอีเมลแอดเดรสถูกต้องหรือไม่เพื่อป้องกันการตีกลับ](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) เมื่อเข้าสู่เครือข่าย Microsoft</span><span class="sxs-lookup"><span data-stu-id="01d4f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="01d4f-104">ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="01d4f-104">Try the following:</span></span>

1. <span data-ttu-id="01d4f-105">ระบุว่าปัญหาเฉพาะเจาะจงกับทั้งโดเมนหรือที่อยู่อีเมลเดียวหรือไม่:</span><span class="sxs-lookup"><span data-stu-id="01d4f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="01d4f-106">โดเมนทั้งหมด: บางครั้งโดเมนจะต้องถูกซิงโครไนซ์ [ลองตั้งค่าโดเมนเป็น ภายใน แล้วกลับไปยัง การเป็นทางการ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="01d4f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="01d4f-107">ที่อยู่อีเมลเดียว: บางครั้งจะต้องซิงโครไนซ์ที่อยู่ การเปลี่ยนที่อยู่พร็อกซี SMTP แล้วเปลี่ยนกลับสามารถช่วยได้</span><span class="sxs-lookup"><span data-stu-id="01d4f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="01d4f-108">ระบุว่าปัญหาเฉพาะเจาะจงกับกลุ่มหรือโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="01d4f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="01d4f-109">วัตถุบางชนิดอาจต้องสร้างวัตถุด้วยตนเองใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="01d4f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="01d4f-110">หากคุณต้องการความช่วยเหลือเพิ่มเติม โปรดเปิดตั๋วการสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงชนิดของวัตถุที่คุณส่งไป) เพื่อให้เราสามารถช่วยเหลือคุณได้ดีขึ้น</span><span class="sxs-lookup"><span data-stu-id="01d4f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>