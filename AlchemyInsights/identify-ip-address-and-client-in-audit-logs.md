---
title: ระบุที่อยู่ IP และไคลเอนต์ในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539048"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>ระบุที่อยู่ IP และไคลเอนต์ในบันทึกการตรวจสอบ

อยู่ IP ที่สอดคล้องกับกิจกรรมที่มีผู้ใช้ Office 365 หรือผู้ดูแล จะปรากฏในบันทึกการตรวจสอบนั้น ไคลเอ็นต์ข้อมูลยังถูกบันทึกไว้ ต่อไปนี้เป็นขั้นตอนเพื่อระบุข้อมูลดังกล่าว

1. เข้าสู่ระบบไปยัง[ศูนย์การปฏิบัติตามกฎระเบียบ & ความปลอดภัย 365 Office](https://protection.office.com/)

2. การ**ค้นหา**ไป > เพ**จค้นหาแฟ้มบันทึกการตรวจสอบ**

   หากคุณสนใจในกิจกรรมหนึ่ง ๆ เลือกค่าจากรายการ**กิจกรรม** ถ้า ไม่มี กิจกรรมทั้งหมดจะถูกส่งกลับสำหรับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)

   **หมายเหตุ**: กิจกรรมบางอย่างอาจไม่พร้อมใช้งานในเมนู**กิจกรรม** อย่างไรก็ตาม ที่ทำการตรวจสอบสินค้าจะถูกส่งกลับถ้า**แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมดที่**ถูกเลือก (ค่าเริ่มต้น)

3. ระบุชื่อผู้ใช้ในฟิลด์**ผู้ใช้**เลือกช่วงวันที่เหมาะสมสำหรับกิจกรรม และจากนั้น คลิก**ค้นหา**

ในผลลัพธ์ คุณสามารถดูอยู่ IP สำหรับกิจกรรมนั้นในบานหน้าต่างผลลัพธ์ เลือกเรกคอร์ดตรวจสอบเพื่อดูข้อมูลรายละเอียดในเมนูลอยขึ้น**รายละเอียด**(ตัวอย่างเช่น ไคลเอ็นต์ ผู้ใช้ที่ทำการดำเนินการ เป็นต้น)

สำหรับข้อมูลเพิ่มเติม ดู[การค้นหาอยู่ IP ของคอมพิวเตอร์ที่ใช้ในการเข้าถึงบัญชีจากการถูกโจมตี](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
