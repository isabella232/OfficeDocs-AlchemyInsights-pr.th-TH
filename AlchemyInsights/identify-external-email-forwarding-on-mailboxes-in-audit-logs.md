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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696316"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>ระบุเวลาที่การส่งต่ออีเมลภายนอกถูกกำหนดค่าในกล่องจดหมาย

เมื่อผู้ใช้ Microsoft ๓๖๕กำหนดค่าการส่งต่ออีเมลภายนอกในกล่องจดหมายกิจกรรมจะถูกตรวจสอบโดยเป็นส่วนหนึ่งของ cmdlet**กล่องจดหมายตั้งค่า** คุณสามารถดูกิจกรรมโดยใช้การค้นหาบันทึกการตรวจสอบในศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย

1. ลงชื่อเข้าใช้[ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)

2. ไปที่หน้า**Search**  >  **ค้นหาบันทึกการตรวจสอบ**การค้นหา

3. เลือกช่วงวันที่ในเขตข้อมูลวันที่**เริ่มต้น**และ**วันที่สิ้นสุด** คุณไม่จำเป็นต้องระบุชื่อผู้ใช้ ตรวจสอบว่าเขตข้อมูล **กิจกรรม** ถูกตั้งค่าให้ **แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด**หรือไม่

4. คลิก**ค้นหา**

ในผลลัพธ์ให้คลิก **ตัวกรองผลลัพธ์** และชนิดของ **กล่องจดหมายตั้งค่า** ในกล่องตัวกรองกิจกรรม เลือกระเบียนการตรวจสอบในผลลัพธ์ ในเมนู**รายละเอียด**ให้คลิก**ข้อมูลเพิ่มเติม** คุณต้องดูรายละเอียดของระเบียนการตรวจสอบแต่ละระเบียนเพื่อกำหนดว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมลหรือไม่

- **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ได้รับการปรับเปลี่ยน

- **พารามิเตอร์**: _ForwardingSmtpAddress_ ระบุที่อยู่อีเมลของเป้าหมาย

- **UserId**: ผู้ใช้ที่กำหนดค่าการส่งต่ออีเมลในกล่องจดหมายในเขตข้อมูล**ObjectId**

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การกำหนดผู้ที่ตั้งค่าการส่งต่ออีเมลสำหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
