---
title: 1332 OWA - กฎของกล่องขาเข้าจะไม่ดำเนินการสำหรับกล่องจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204079"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>กฎของกล่องขาเข้าไม่ทำงานตามที่คาดไว้

ตรวจสอบการตั้งค่าต่อไปนี้:

- ข้อความสามารถถูกเปลี่ยนเส้นทาง ส่งต่อ หรือโดยอัตโนมัติขึ้นอยู่กับกฎของกล่องขาเข้าเพียงครั้งเดียวเรียบร้อยแล้ว กฎการเปลี่ยนทิศทาง (ผิดกฎของกล่องขาเข้าหรือกระแสกฎสำหรับจดหมาย หรือที่เรียกอีกอย่างหนึ่งว่ากฎการขนส่ง) สามารถเพิ่มได้สูงสุดสิบการผู้รับส่งต่อข้อความ สำหรับข้อมูลเพิ่มเติม ให้ดู[สมุดรายวัน ขน ส่ง และอินบ็อกซ์ขีดจำกัดกฎ](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- กฎของกล่องขาเข้าไม่ทำงานกับกล่องจดหมายอื่นบันทึกนั้น สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายบันทึกสำรอง ดู[กล่องจดหมายบันทึกสำรอง](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

เมื่อต้องการแก้ไขปัญหาเหล่านี้ ดู[KB 2829319](https://support.microsoft.com/kb/2829319)

ถ้าไม่สามารถใช้กับปัญหาก่อนหน้านี้ เรียกใช้การวินิจฉัยรายงานกฎกล่องขาเข้าก่อนที่คุณเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของ Microsoft:

1. เปิดกล่องจดหมายใน Outlook บนเว็บ และคลิก <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **การตั้งค่า** > **ดูการตั้งค่า Outlook ทั้งหมด** > **เม** > **กฎ**

2. ที่ด้านล่างของหน้า คลิก**ถ้ากฎของคุณกำลังทำงานอยู่ให้คลิกที่นี่เพื่อสร้างรายงานการวินิจฉัย**
