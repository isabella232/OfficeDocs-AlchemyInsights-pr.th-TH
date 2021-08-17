---
title: 1332 OWA - กฎของกล่องจดหมายเข้าจะไม่ประมวลผลในกล่องจดหมาย
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040921"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>กฎกล่องจดหมายเข้าไม่ได้ผลตามที่คาดไว้

ตรวจสอบการตั้งค่าต่อไปนี้ในOutlook บนเว็บ:

- สามารถเปลี่ยนเส้นทาง ส่งต่อ หรือตอบกลับข้อความโดยอัตโนมัติโดยยึดตามกฎของกล่องจดหมายเข้าได้เพียงหนึ่งครั้งเท่านั้น กฎการเปลี่ยนเส้นทาง (กฎของกล่องจดหมายเข้าหรือกฎของลเป้าหมาย หรือที่เรียกว่ากฎการส่งผ่าน) สามารถเพิ่มผู้รับที่ส่งต่อได้สูงสุด 10 คนลงในข้อความได้ For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- กฎกล่องจดหมายเข้าไม่สามารถใช้งานกับกล่องจดหมายบันทึกอื่นได้ For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

เมื่อต้องการแก้ไขปัญหาเหล่านี้ [ให้ดู](https://support.microsoft.com/kb/2829319)2829319 KB

ถ้าปัญหาก่อนหน้านี้ใช้ไม่ได้ ให้เรียกใช้รายงานการวินิจฉัยกฎของกล่องจดหมายเข้าก่อนที่คุณจะแจ้งปัญหาไปยังฝ่ายสนับสนุนของ Microsoft:

1. เปิดกล่องจดหมายOutlook บนเว็บ แล้วคลิก <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **การตั้งค่า**  >  **ดูทั้งหมด Outlook การตั้งค่า**  >  **จดหมาย**  >  **กฎ**

2. ที่ด้านล่างของหน้า ให้คลิก ถ้า **กฎของคุณไม่พร้อมให้ใช้งาน คลิกที่นี่เพื่อสร้างรายงาน** การวินิจฉัย
