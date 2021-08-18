---
title: ระบุเหตุการณ์การลบข้อความในบันทึกการตรวจสอบ
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317613"
---
# <a name="audit-logs-for-deleted-email-messages"></a>ตรวจสอบบันทึกของข้อความอีเมลที่ถูกลบ

ตั้งแต่เดือนมกราคม 2019 Microsoft จะเปิดใช้งานบันทึกการตรวจสอบกล่องจดหมายตามค่าเริ่มต้น มิฉะนั้น เมื่อต้องการตรวจสอบเหตุการณ์การลบข้อความของผู้ใช้เฉพาะ คุณจึงต้องเปิดใช้งานการลบด้วยตนเองเพื่อการตรวจสอบ ถ้าบันทึกการตรวจสอบกล่องจดหมายถูกเปิดใช้งานอยู่แล้วในองค์กรของคุณหรือผู้ใช้ที่ระบุ ให้ปฏิบัติตามขั้นตอนด้านล่าง

1. เข้าสู่ระบบศูนย์การปฏิบัติตาม[Microsoft 365มาตรฐาน](https://protection.office.com/)

2. คลิก **ค้นหาและตรวจสอบ****แล้วเลือก การค้นหาบันทึก** การตรวจสอบ

3. เลือกช่วงวันที่ในเขตข้อมูล **วันที่เริ่มต้น****และ** วันที่สิ้นสุด ระบุชื่อผู้ใช้ของผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ) ใน **เขตข้อมูลกิจกรรม** ให้เลือก ข้อความ **ที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ****และ ย้ายข้อความไปยังโฟลเดอร์รายการ** ที่ถูกลบ

4. **คลิก** ค้นหา

ในผลลัพธ์ ให้เลือกระเบียนการตรวจสอบ ในฟลายเอาท์รายละเอียด **ให้คลิก** ข้อมูลเพิ่มเติม ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ (ตัวอย่างเช่น บรรทัดเรื่องและที่ตั้งของรายการเมื่อรายการถูกลบ) จะแสดงอยู่ใน **เขตข้อมูล AffectedItems** คุณสมบัติ **ClientInfoString** จะแสดงถ้าการลบเกิดขึ้นใน Outlook, Outlook บนเว็บ (เดิมเรียกว่า Outlook Web App) หรืออุปกรณ์อื่นๆ

For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**หมายเหตุ**: คุณไม่สามารถเรียกใช้รายการที่ถูกลบโดยใช้ฟีเจอร์บันทึกการตรวจสอบได้ เมื่อต้องการเรียกใช้ข้อความที่ถูกลบOutlook บนเว็บ ดู[กู้คืนรายการที่ถูกลบใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
