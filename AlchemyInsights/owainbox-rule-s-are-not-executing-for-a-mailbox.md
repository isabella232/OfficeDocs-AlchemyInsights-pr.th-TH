---
title: 1332 OWA - กฎกล่องขาเข้าจะไม่ดําเนินการสําหรับกล่องจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576579"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>กฎกล่องขาเข้าไม่ทํางานตามที่คาดไว้

ตรวจสอบการตั้งค่าต่อไปนี้ใน Outlook บนเว็บ:

- ข้อความสามารถเปลี่ยนเส้นทาง ส่งต่อ หรือตอบกลับโดยอัตโนมัติตามกฎของกล่องขาเข้าเพียงครั้งเดียว กฎการเปลี่ยนเส้นทาง (กฎกล่องขาเข้าหรือกฎการรับส่งจดหมาย หรือที่เรียกว่ากฎการขนส่ง) สามารถเพิ่มผู้รับการส่งต่อได้สูงสุดสิบคนในข้อความ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ขีดจํากัดกฎสมุดรายวัน การขนส่ง และกล่องขาเข้า](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- กฎของกล่องขาเข้าไม่ทํางานบนกล่องจดหมายบันทึกอื่น สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายบันทึกประจําวันอื่น ให้ดูที่[กล่องจดหมายบันทึกอื่น](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

เมื่อต้องการแก้ไขปัญหาเหล่านี้ ให้ดูที่[KB 2829319](https://support.microsoft.com/kb/2829319)

ถ้าปัญหาก่อนหน้านี้ไม่ได้ใช้ เรียกใช้รายงานการวินิจฉัยกฎกล่องขาเข้าก่อนที่คุณเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของ Microsoft:

1. เปิดกล่องจดหมายใน Outlook บนเว็บ และคลิก <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **การตั้งค่า**  >  **ดูการตั้งค่า**  >  Outlook ทั้งหมด **จดหมาย**  >  **กฎ**

2. ที่ด้านล่างของหน้า ให้คลิก**ถ้ากฎของคุณไม่ทํางาน ให้คลิก ที่นี่ เพื่อสร้างรายงานการวินิจฉัย**
