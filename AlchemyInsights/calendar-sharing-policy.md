---
title: นโยบายการแชร์ปฏิทินของ๖๑๘
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684249"
---
# <a name="policy-error-when-sharing-a-calendar"></a>ข้อผิดพลาดของนโยบายเมื่อแชร์ปฏิทิน

1. ให้เลือกทำอย่างใดอย่างหนึ่งต่อไปนี้ตามความเหมาะสมกับสถานการณ์ของคุณ:
    - เชื่อมต่อกับ Exchange Online โดยใช้ PowerShell ระยะไกล สำหรับข้อมูลเพิ่มเติมให้ดู[ที่เชื่อมต่อกับ Exchange Online โดยใช้ PowerShell ระยะไกล](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - บนเซิร์ฟเวอร์ภายในองค์กรให้เปิดเชลล์การจัดการ Exchange
2. กำหนดนโยบายการแชร์ที่มอบหมายให้กับผู้ใช้ เมื่อต้องการทำเช่นนี้ให้เรียกใช้คำสั่งต่อไปนี้และบันทึกนโยบายที่ส่งกลับ:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. อัปเดตกโยบายการแชร์สำหรับผู้ใช้ เมื่อต้องการทำเช่นนี้ให้ทำตามขั้นตอนต่อไปนี้:
    - เปิดศูนย์การจัดการ Exchange
    - คลิก**องค์กร**แล้วดับเบิลคลิกที่นโยบายที่กำหนดให้กับผู้ใช้ภายใต้การ**แชร์แต่ละรายการ** นี่คือนโยบายที่ส่งกลับในขั้นตอนที่2
    - บนหน้ากฎการแชร์ให้เลือกระดับการแชร์ปฏิทินที่คุณต้องการอนุญาตภายใต้**ระบุข้อมูลที่คุณต้องการแชร์** คลิก**บันทึก**

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่: "นโยบายไม่อนุญาตให้สิทธิ์ในระดับนี้ไปยังข้อผิดพลาดของผู้รับอย่างน้อยหนึ่งข้อผิดพลาด" เมื่อผู้ใช้พยายามแชร์ปฏิทิน](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
