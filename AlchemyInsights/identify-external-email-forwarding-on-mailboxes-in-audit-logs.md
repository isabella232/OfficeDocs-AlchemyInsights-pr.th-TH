---
title: ระบุการส่งต่ออีเมภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539120"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>ระบุเมื่อมีการกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย

เมื่อผู้ใช้ Office 365 สามารถกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย กิจกรรมที่กำลังตรวจสอบเป็นส่วนหนึ่งของการ cmdlet**กล่องจดหมายชุด** คุณสามารถดูกิจกรรมที่ใช้ค้นหาแฟ้มบันทึกการตรวจสอบใน & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ

1. เข้าสู่ระบบไปยัง[ศูนย์การปฏิบัติตามกฎระเบียบ & ความปลอดภัย 365 Office](https://protection.office.com/)

2. การ**ค้นหา**ไป > เพ**จค้นหาแฟ้มบันทึกการตรวจสอบ**

3. เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด** คุณไม่จำเป็นเมื่อต้องการระบุชื่อผู้ใช้ ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเพื่อ**แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด**

4. คลิก**ค้นหา**

ในผลลัพธ์**ผลลัพธ์ของตัวกรอง**คลิก และพิมพ์การ**ตั้งค่าจดหมาย**ในกล่องตัวกรองกิจกรรม เลือกเรกคอร์ดที่มีตรวจสอบในผลลัพธ์ ในเมนูลอยขึ้น**รายละเอียด**คลิ**กข้อมูลเพิ่มเติม** คุณต้องดูที่รายละเอียดของแต่ละระเบียนตรวจสอบเพื่อตรวจสอบว่า กิจกรรมที่เกี่ยวข้องเพื่อส่งต่ออีเมล

- **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน

- **พารามิเตอร์**: _ForwardingSmtpAddress_บ่งชี้ว่า อยู่อีเมลของเป้าหมาย

- **UserId**: ผู้ใช้ที่กำหนดค่าไว้ส่งต่ออีเมลในกล่องจดหมายในฟิลด์**ObjectId**

สำหรับข้อมูลเพิ่มเติม ดู[Determining ที่ติดตั้งอีเมลที่ส่งต่อสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)
