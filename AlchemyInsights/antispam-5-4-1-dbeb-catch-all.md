---
title: การป้องกันสแปม 5.4.1 DBEB จับทั้งหมด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964347"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>แก้ไขปัญหาการจัดส่งสำหรับรหัสข้อผิดพลาด๕๕๐5.4.1 การเข้าถึงรีเลย์ถูกปฏิเสธ

ปัญหานี้เกิดขึ้นเมื่อ[ตรวจสอบเพื่อดูว่าที่อยู่ e-mail ถูกต้องเพื่อป้องกันไม่ให้ bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)เมื่อเข้าสู่เครือข่าย Office ๓๖๕ ลองทำดังต่อไปนี้:

1. ตรวจสอบว่าปัญหามีความเฉพาะเจาะจงสำหรับทั้งโดเมนหรือที่อยู่เดียว:
    - โดเมนทั้งหมด: บางครั้งโดเมนต้องทำข้อมูลให้ตรงกัน ลอง[ตั้งค่าโดเมนเป็น "ภายใน" แล้วกลับไปที่](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)สิทธิ์
     - ที่อยู่เดียว: บางครั้งที่อยู่จะต้องมีการทำข้อมูลให้ตรงกัน การเปลี่ยนแปลงที่อยู่พร็อกซี smtp และจากนั้นเปลี่ยนกลับสามารถช่วย
2. ตรวจสอบว่าปัญหาที่เกิดขึ้นเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะ วัตถุบางชนิดอาจต้องถูกสร้างด้วยตนเองในไดเรกทอรีที่ใช้งานอยู่ของ Azure

หากคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดตั๋วสนับสนุนและระบุขอบเขตของปัญหา (includidng ชนิดของวัตถุที่คุณกำลังส่งไป) เพื่อให้เราสามารถช่วยให้คุณได้ดียิ่งขึ้น