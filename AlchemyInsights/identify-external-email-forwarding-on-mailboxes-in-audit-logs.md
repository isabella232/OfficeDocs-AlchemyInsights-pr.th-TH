---
title: ระบุการส่งต่ออีเมภายนอกบนกล่องจดหมายในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909625"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>ระบุเมื่อมีการกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย

เมื่อผู้ใช้สามารถกำหนดค่าการส่งต่ออีเมภายนอกบนกล่องจดหมาย กิจกรรมที่กำลังตรวจสอบเป็นส่วนหนึ่งของการ cmdlet**กล่องจดหมายชุด** คุณสามารถดูกิจกรรมที่ใช้ค้นหาแฟ้มบันทึกการตรวจสอบใน & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ

1. เข้าสู่ระบบไปยัง[ศูนย์ปฏิบัติตามกฎระเบียบ & 365 ความปลอดภัยของ Office](https://protection.office.com/)

2. คลิก**ค้นหาและการตรวจสอบ**และ**ค้นหาแฟ้มบันทึกการตรวจสอบบัญชี**ที่เลือก

3. เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด** คุณไม่จำเป็นเมื่อต้องการระบุชื่อผู้ใช้ ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเพื่อ**แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด**

4. คลิก**ค้นหา**

ในผลลัพธ์**ผลลัพธ์ของตัวกรอง**คลิก และพิมพ์การ**ตั้งค่าจดหมาย**ในกล่องตัวกรองกิจกรรม เลือกเรกคอร์ดที่มีตรวจสอบในผลลัพธ์ ในเมนูลอยขึ้น**รายละเอียด**คลิ**กข้อมูลเพิ่มเติม** คุณต้องดูที่รายละเอียดของแต่ละระเบียนตรวจสอบเพื่อตรวจสอบว่า กิจกรรมที่เกี่ยวข้องเพื่อส่งต่ออีเมล

- **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน

- **พารามิเตอร์**: _ForwardingSmtpAddress_บ่งชี้ว่า อยู่อีเมลของเป้าหมาย

- **UserId**: ผู้ใช้ที่กำหนดค่าไว้ส่งต่ออีเมลในกล่องจดหมายในฟิลด์**ObjectId**

สำหรับข้อมูลเพิ่มเติม ดู[Determining ที่ติดตั้งอีเมลที่ส่งต่อสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)
