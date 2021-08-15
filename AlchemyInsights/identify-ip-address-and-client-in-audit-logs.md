---
title: ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014919"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ

ที่อยู่ IP ที่สอดคล้องกับกิจกรรมโดยผู้ใช้Microsoft 365ผู้ดูแลระบบจะแสดงในบันทึกการตรวจสอบ ข้อมูลไคลเอ็นต์จะได้รับการบันทึกด้วย ต่อไปนี้เป็นขั้นตอนในการระบุข้อมูลดังกล่าว

1. เข้าสู่ระบบศูนย์การปฏิบัติตาม[Microsoft 365มาตรฐาน](https://protection.office.com/)

2. ไปที่หน้า  >  **ค้นหาบันทึกการตรวจสอบ** การค้นหา

   ถ้าคุณสนใจกิจกรรมที่เฉพาะเจาะจง ให้เลือก **กิจกรรมจากรายการ** กิจกรรม ถ้าไม่ กิจกรรมทั้งหมดจะถูกส่งกลับให้กับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)

   **หมายเหตุ**: บางกิจกรรมอาจไม่พร้อมใช้งาน **ในเมนูกิจกรรม** อย่างไรก็ตาม รายการตรวจสอบเหล่านั้นจะถูกส่งกลับถ้า **เลือก แสดงผลลัพธ์ให้กับกิจกรรม** ทั้งหมด (การตั้งค่าเริ่มต้น)

3. ระบุ **ชื่อผู้ใช้ในเขตข้อมูล** ผู้ใช้ เลือกช่วงวันที่ที่เหมาะสมของกิจกรรม **จากนั้นคลิก** ค้นหา

ในผลลัพธ์ คุณสามารถดูที่อยู่ IP ของกิจกรรมนั้นในบานหน้าต่างผลลัพธ์ เลือกระเบียนการตรวจสอบเพื่อดูข้อมูลโดยละเอียดใน **แถบ** ฟลายเอาท์ รายละเอียด (ตัวอย่างเช่น ไคลเอ็นต์ ผู้ใช้ที่ได้ปฏิบัติการฯลฯ)

For more information, see [Finding the IP address of the computer used to access a compromised account](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
