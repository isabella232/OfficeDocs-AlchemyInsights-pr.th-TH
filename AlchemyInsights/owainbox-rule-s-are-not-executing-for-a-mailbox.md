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
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>กฎกล่องจดหมายเข้าไม่ทำงานตามที่คาดไว้

ตรวจสอบการตั้งค่าต่อไปนี้ใน Outlook บนเว็บ:

- ข้อความสามารถถูกเปลี่ยนเส้นทางส่งต่อหรือตอบกลับโดยอัตโนมัติโดยยึดตามกฎของกล่องจดหมายเข้าได้เพียงครั้งเดียวเท่านั้น กฎการเปลี่ยนเส้นทาง (กฎของกล่องขาเข้าหรือกฎการไหลของจดหมายหรือที่เรียกว่ากฎการขนส่ง) สามารถเพิ่มผู้รับการส่งต่อได้สูงสุดสิบรายไปยังข้อความ สำหรับข้อมูลเพิ่มเติมให้ดูที่[ขีดจำกัดของสมุดบันทึกการขนส่งและกฎของกล่องจดหมายเข้า](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- กฎของกล่องจดหมายเข้าไม่ทำงานบนกล่องจดหมายการบันทึกอื่น สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายการบันทึกอื่นให้ดูที่[กล่องจดหมายการบันทึกอื่น](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

เมื่อต้องการแก้ไขปัญหาเหล่านี้ให้ดู[KB ๒๘๒๙๓๑๙](https://support.microsoft.com/kb/2829319)

ถ้าปัญหาก่อนหน้านี้ไม่ได้นำไปใช้ให้เรียกใช้รายงานการวินิจฉัยกฎของกล่องจดหมายเข้าก่อนที่คุณจะเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของไมโครซอฟท์:

1. เปิดกล่องจดหมายใน Outlook บนเว็บแล้วคลิก <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **การตั้งค่า**  >  **ดูการตั้งค่า**  >  Outlook ทั้งหมด **จดหมาย**  >  **กฎ**

2. ที่ด้านล่างของหน้าให้คลิก**ถ้ากฎของคุณไม่ทำงานให้คลิกที่นี่เพื่อสร้างรายงานการวินิจฉัย**
