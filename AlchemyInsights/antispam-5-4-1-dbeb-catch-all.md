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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>แก้ไขปัญหาการส่งรหัสข้อผิดพลาด 550 5.4.1 การเข้าถึงรีเลย์ถูกปฏิเสธ

ปัญหานี้เกิดขึ้นเมื่อ [ตรวจสอบเพื่อดูว่าอีเมลแอดเดรสถูกต้องหรือไม่เพื่อป้องกันการตีกลับ](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) เมื่อเข้าสู่เครือข่าย Microsoft ลองวิธีต่อไปนี้:

1. ระบุว่าปัญหาเฉพาะเจาะจงกับทั้งโดเมนหรือที่อยู่อีเมลเดียวหรือไม่:
    - โดเมนทั้งหมด: บางครั้งโดเมนจะต้องถูกซิงโครไนซ์ [ลองตั้งค่าโดเมนเป็น ภายใน แล้วกลับไปยัง การเป็นทางการ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - ที่อยู่อีเมลเดียว: บางครั้งจะต้องซิงโครไนซ์ที่อยู่ การเปลี่ยนที่อยู่พร็อกซี SMTP แล้วเปลี่ยนกลับสามารถช่วยได้
2. ระบุว่าปัญหาเฉพาะเจาะจงกับกลุ่มหรือโฟลเดอร์สาธารณะ วัตถุบางชนิดอาจต้องสร้างวัตถุด้วยตนเองใน Azure Active Directory

หากคุณต้องการความช่วยเหลือเพิ่มเติม โปรดเปิดตั๋วการสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงชนิดของวัตถุที่คุณส่งไป) เพื่อให้เราสามารถช่วยเหลือคุณได้ดีขึ้น