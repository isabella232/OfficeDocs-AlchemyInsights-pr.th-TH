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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932296"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>แก้ไขปัญหาการส่งรหัสข้อผิดพลาด 550 5.4.1 การเข้าถึงรีเลย์ถูกปฏิเสธ

ปัญหานี้เกิดขึ้นเมื่อ [ตรวจสอบเพื่อดูว่าอีเมลแอดเดรสถูกต้องหรือไม่เพื่อป้องกันการตีกลับ](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) เมื่อเข้าสู่เครือข่าย Microsoft ลองวิธีต่อไปนี้:

1. ระบุว่าปัญหาเฉพาะเจาะจงกับทั้งโดเมนหรือที่อยู่อีเมลเดียวหรือไม่:
    - โดเมนทั้งหมด: บางครั้งโดเมนจะต้องถูกซิงโครไนซ์ [ลองตั้งค่าโดเมนเป็น ภายใน แล้วกลับไปยัง การเป็นทางการ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - ที่อยู่อีเมลเดียว: บางครั้งจะต้องซิงโครไนซ์ที่อยู่ การเปลี่ยนที่อยู่พร็อกซี SMTP แล้วเปลี่ยนกลับสามารถช่วยได้
2. ระบุว่าปัญหาเฉพาะเจาะจงกับกลุ่มหรือโฟลเดอร์สาธารณะ วัตถุบางชนิดอาจต้องสร้างขึ้นด้วยตนเองในวัตถุAzure Active Directoryวัตถุ

หากคุณต้องการความช่วยเหลือเพิ่มเติม โปรดเปิดตั๋วการสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงชนิดของวัตถุที่คุณส่งไป) เพื่อให้เราสามารถช่วยเหลือคุณได้ดีขึ้น