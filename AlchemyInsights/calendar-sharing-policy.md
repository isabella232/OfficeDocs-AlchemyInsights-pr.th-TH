---
title: นโยบายการแชร์ปฏิทิน 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373018"
---
# <a name="policy-error-when-sharing-a-calendar"></a>ข้อผิดพลาดนโยบายเมื่อแชร์ปฏิทิน

1. ทําอย่างใดอย่างหนึ่งต่อไปนี้ ตามความเหมาะสมกับสถานการณ์ของคุณ:
    - เชื่อมต่อกับอัตราแลกเปลี่ยนแบบออนไลน์ โดยใช้ PowerShell ระยะไกล สําหรับข้อมูลเพิ่มเติม ให้ดู[การเชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์โดยใช้ PowerShell ระยะไกล](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - บนเซิร์ฟเวอร์ในสถานที่เปิดเชลล์จัดการการแลกเปลี่ยน
2. กําหนดนโยบายการใช้ร่วมกันที่กําหนดให้กับผู้ใช้ เรียกใช้คําสั่งต่อไปนี้ และหมายเหตุนโยบายที่ส่งคืน:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. ปรับปรุงนโยบายการใช้ร่วมกันสําหรับผู้ใช้ เมื่อต้องการทําเช่นนี้ ให้ทําตามขั้นตอนเหล่านี้:
    - เปิดศูนย์การจัดการ Exchange
    - คลิก**องค์กร**แล้วคลิกสองครั้งที่นโยบายที่กําหนดให้กับผู้ใช้ภายใต้**การแชร์แต่ละบุคคล** นี่คือนโยบายที่ถูกส่งกลับในขั้นตอนที่ 2
    - บนหน้า กฎการแชร์ ให้เลือกระดับการแชร์ปฏิทินที่คุณต้องการ**อนุญาตภายใต้** คลิก**บันทึก**

สําหรับข้อมูลเพิ่มเติม ให้ดู: ["นโยบายไม่อนุญาตให้ให้สิทธิ์ที่ระดับนี้ไปยังผู้รับอย่างน้อยหนึ่งข้อผิดพลาด"เมื่อผู้ใช้พยายามใช้ปฏิทินร่วมกัน](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
