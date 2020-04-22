---
title: ป้องกันสแปม 5.4.1 DBEB จับทั้งหมด
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707930"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>แก้ไขปัญหาการจัดส่งสําหรับรหัสข้อผิดพลาด 550 5.4.1 Relay Access ถูกปฏิเสธ

ปัญหานี้เกิดขึ้นเมื่อ[ตรวจสอบเพื่อดูว่า อยู่อีเมลถูกต้องเพื่อป้องกัน bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)เมื่อเข้าสู่เครือข่ายของ Microsoft ลองทําดังนี้

1. ตรวจสอบว่า ปัญหาเฉพาะกับโดเมนทั้งหมดหรือที่อยู่อีเมลเดียว:
    - โดเมนทั้งหมด: บางครั้งโดเมนต้องถูกซิงโครไนซ์ ลอง[ตั้งค่าโดเมนเป็นภายในแล้วกลับไปที่ Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - ที่อยู่อีเมลเดียว: บางครั้งที่อยู่จะต้องมีการซิงโครไนซ์ การเปลี่ยนที่อยู่พร็อกซี SMTP แล้วเปลี่ยนกลับสามารถช่วย
2. ตรวจสอบว่า ปัญหาเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะ สําหรับบางชนิดวัตถุ วัตถุอาจจําเป็นต้องถูกสร้างด้วยตนเองในไดเรกทอรีที่ใช้งานอยู่ของ Azure

หากคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดตั๋วสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงประเภทของวัตถุที่คุณกําลังส่งไป) เพื่อให้เราสามารถช่วยให้คุณดีขึ้น