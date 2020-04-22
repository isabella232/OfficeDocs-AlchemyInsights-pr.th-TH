---
title: ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716407"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ

อยู่ IP ที่สอดคล้องกับกิจกรรม โดยผู้ใช้ Microsoft 365 หรือผู้ดูแลระบบจะแสดงในบันทึกการตรวจสอบ ข้อมูลไคลเอ็นต์จะถูกบันทึกด้วย ต่อไปนี้เป็นขั้นตอนในการระบุข้อมูลดังกล่าว

1. เข้าสู่ระบบศูนย์[การปฏิบัติตาม&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)

2. ไปที่หน้า**ค้นหาบันทึกการตรวจสอบ****การค้นหา** > 

   ถ้าคุณสนใจกิจกรรมเฉพาะ ให้เลือกกิจกรรมจากรายการ**กิจกรรม** ถ้าไม่ กิจกรรมทั้งหมดจะถูกส่งกลับสําหรับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)

   **หมายเหตุ**: กิจกรรมบางอย่างอาจไม่มีในเมนู**กิจกรรม** อย่างไรก็ตาม รายการการตรวจสอบเหล่านั้นจะถูกส่งกลับถ้า**แสดงผลลัพธ์สําหรับกิจกรรมทั้งหมด**ถูกเลือกไว้ (การตั้งค่าเริ่มต้น)

3. ระบุชื่อผู้ใช้ในฟิลด์**ผู้ใช้**ให้เลือกช่วงวันที่ที่เหมาะสมสําหรับกิจกรรม แล้วคลิก**ค้นหา**

ในผลลัพธ์ คุณจะเห็นที่อยู่ IP สําหรับกิจกรรมนั้นในบานหน้าต่างผลลัพธ์ เลือกเรกคอร์ดการตรวจสอบเพื่อดูข้อมูลโดยละเอียด**ในรายละเอียดลอย**(ตัวอย่างเช่น ลูกค้า ผู้ใช้ที่ดําเนินการ กระทํา ฯลฯ)

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การค้นหาที่อยู่ IP ของคอมพิวเตอร์ที่ใช้ในการเข้าถึงบัญชีที่ถูกบุกรุก](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
