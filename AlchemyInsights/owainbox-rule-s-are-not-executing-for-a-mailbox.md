---
title: ๑๓๓๒ OWA-กฎกล่องจดหมายเข้าจะไม่ดำเนินการสำหรับกล่องจดหมาย
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721610"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="2bb35-102">กฎกล่องจดหมายเข้าไม่ทำงานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="2bb35-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="2bb35-103">ตรวจสอบการตั้งค่าต่อไปนี้ใน Outlook บนเว็บ:</span><span class="sxs-lookup"><span data-stu-id="2bb35-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="2bb35-104">ข้อความสามารถถูกเปลี่ยนเส้นทางส่งต่อหรือตอบกลับโดยอัตโนมัติโดยยึดตามกฎของกล่องจดหมายเข้าได้เพียงครั้งเดียวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="2bb35-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="2bb35-105">กฎการเปลี่ยนเส้นทาง (กฎของกล่องขาเข้าหรือกฎการไหลของจดหมายหรือที่เรียกว่ากฎการขนส่ง) สามารถเพิ่มผู้รับการส่งต่อได้สูงสุดสิบรายไปยังข้อความ</span><span class="sxs-lookup"><span data-stu-id="2bb35-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="2bb35-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ขีดจำกัดของสมุดบันทึกการขนส่งและกฎของกล่องจดหมายเข้า](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)</span><span class="sxs-lookup"><span data-stu-id="2bb35-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="2bb35-107">กฎของกล่องจดหมายเข้าไม่ทำงานบนกล่องจดหมายการบันทึกอื่น</span><span class="sxs-lookup"><span data-stu-id="2bb35-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="2bb35-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายการบันทึกอื่นให้ดูที่[กล่องจดหมายการบันทึกอื่น](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)</span><span class="sxs-lookup"><span data-stu-id="2bb35-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="2bb35-109">เมื่อต้องการแก้ไขปัญหาเหล่านี้ให้ดู[KB ๒๘๒๙๓๑๙](https://support.microsoft.com/kb/2829319)</span><span class="sxs-lookup"><span data-stu-id="2bb35-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="2bb35-110">ถ้าปัญหาก่อนหน้านี้ไม่ได้นำไปใช้ให้เรียกใช้รายงานการวินิจฉัยกฎของกล่องจดหมายเข้าก่อนที่คุณจะเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของไมโครซอฟท์:</span><span class="sxs-lookup"><span data-stu-id="2bb35-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="2bb35-111">เปิดกล่องจดหมายใน Outlook บนเว็บแล้วคลิก</span><span class="sxs-lookup"><span data-stu-id="2bb35-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="2bb35-112">**การตั้งค่า**  >  **ดูการตั้งค่า**  >  Outlook ทั้งหมด **จดหมาย**  >  **กฎ**</span><span class="sxs-lookup"><span data-stu-id="2bb35-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="2bb35-113">ที่ด้านล่างของหน้าให้คลิก**ถ้ากฎของคุณไม่ทำงานให้คลิกที่นี่เพื่อสร้างรายงานการวินิจฉัย**</span><span class="sxs-lookup"><span data-stu-id="2bb35-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
