---
title: ระบุการส่งต่ออีเมลภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028774"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>ระบุเมื่อการส่งต่ออีเมลภายนอกถูกกําหนดค่าบนกล่องจดหมาย

When a Microsoft 365 configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet. คุณสามารถดูกิจกรรมได้โดยใช้การค้นหาบันทึกการตรวจสอบใน ศูนย์การรักษา&การปฏิบัติตามข้อบังคับ

1. เข้าสู่ระบบศูนย์การปฏิบัติตาม[Microsoft 365มาตรฐาน](https://protection.office.com/)

2. ไปที่หน้า  >  **ค้นหาบันทึกการตรวจสอบ** การค้นหา

3. เลือกช่วงวันที่ในเขตข้อมูล **วันที่เริ่มต้น****และ** วันที่สิ้นสุด คุณไม่ต้ดต้องระบุชื่อผู้ใช้ ตรวจสอบว่า **เขตข้อมูล กิจกรรม** ถูกตั้งค่าเป็น **แสดงผลลัพธ์ให้กับกิจกรรม** ทั้งหมด

4. **คลิก** ค้นหา

ในผลลัพธ์ ให้คลิก **กรองผลลัพธ์** แล้วพิมพ์ **Set-Mailbox** ในกล่องตัวกรองกิจกรรม เลือกระเบียนการตรวจสอบในผลลัพธ์ ใน **ฟลาย** เอาท์ รายละเอียด **ให้คลิก** ข้อมูลเพิ่มเติม คุณต้องดูรายละเอียดของระเบียนการตรวจสอบแต่ละระเบียนเพื่อระบุว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมลหรือไม่

- **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน

- **พารามิเตอร์**: _ForwardingSmtpAddress_ จะระบุที่อยู่อีเมลเป้าหมาย

- **UserId:** ผู้ใช้ที่กําหนดค่าการส่งต่ออีเมลบนกล่องจดหมายใน **เขตข้อมูล ObjectId**

For more information, see [Determining who set up email forwarding for a mailbox](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
