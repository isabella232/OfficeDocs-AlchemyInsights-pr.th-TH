---
title: 618 นโยบายการแชร์ปฏิทิน
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091628"
---
# <a name="policy-error-when-sharing-a-calendar"></a>ข้อผิดพลาดของนโยบายเมื่อแชร์ปฏิทิน

1. เลือกอย่างใดอย่างหนึ่งต่อไปนี้ตามความเหมาะสมกับสถานการณ์ของคุณ
    - เชื่อมต่อ Exchange Online โดยใช้ PowerShell ระยะไกล For more information, see[เชื่อมต่อ Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - บนเซิร์ฟเวอร์ภายในองค์กร ให้เปิด Exchange Management Shell
2. ระบุนโยบายการแชร์ที่มอบหมายให้กับผู้ใช้ เมื่อต้องการเรียกใช้การสั่งต่อไปนี้ และโปรดสังเกตว่านโยบายถูกส่งกลับ:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. อัปเดตนโยบายการแชร์ของผู้ใช้ เมื่อต้องการให้ปฏิบัติตามขั้นตอนเหล่านี้:
    - เปิด Exchangeการจัดการระบบ
    - **คลิก** องค์กร แล้วดับเบิลคลิกนโยบายที่มอบหมายให้กับผู้ใช้ภายใต้ **การแชร์แต่ละรายการ** นี่คือนโยบายที่ถูกส่งกลับในขั้นตอนที่ 2
    - บนหน้า กฎการแชร์ ให้เลือกระดับการแชร์ปฏิทินที่คุณต้องการอนุญาต **ภายใต้ ระบุข้อมูลที่คุณต้องการแชร์** **คลิก** บันทึก

For more information see: ["Policy does not allowing permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
