---
title: แอนตี้สแปม 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717380"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>แก้ไขปัญหาการนำส่งสำหรับรหัสข้อผิดพลาด๕๕๐5.4.1 การเข้าถึงรีเลย์ที่ถูกปฏิเสธ

ปัญหานี้เกิดขึ้นเมื่อ [ตรวจสอบเพื่อดูว่าที่อยู่อีเมลไม่ถูกต้องในการป้องกันไม่ให้ bouncebacks เมื่อเข้า](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) สู่เครือข่าย Microsoft ให้ลองทำดังต่อไปนี้:

1. ตรวจสอบว่าปัญหาเฉพาะกับโดเมนทั้งหมดหรือที่อยู่อีเมลเดียว:
    - โดเมนทั้งหมด: บางครั้งจำเป็นต้องซิงโครไนซ์โดเมน ลอง[ตั้งค่าโดเมนเป็นภายในแล้วกลับไปยังสิทธิ์](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - อีเมลแอดเดรสเดียว: บางครั้งจำเป็นต้องซิงโครไนซ์ที่อยู่ การเปลี่ยนที่อยู่พร็อกซีของ smtp แล้วการเปลี่ยนกลับจะช่วยให้คุณสามารถช่วยได้
2. ตรวจสอบว่าปัญหาเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะหรือไม่ สำหรับชนิดของวัตถุบางชนิดวัตถุอาจจำเป็นต้องถูกสร้างขึ้นด้วยตนเองใน Azure Active Directory

ถ้าคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดบัตรสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงชนิดของวัตถุที่คุณกำลังส่งไป) เพื่อให้เราสามารถช่วยคุณได้ดียิ่งขึ้น