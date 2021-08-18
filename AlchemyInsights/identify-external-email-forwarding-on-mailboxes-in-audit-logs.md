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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331178"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>ระบุเมื่อการส่งต่ออีเมลภายนอกถูกกําหนดค่าบนกล่องจดหมาย

When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet. คุณสามารถดูกิจกรรมได้โดยใช้การค้นหาบันทึกการตรวจสอบ วิธีการ:

1. ให้เลือกปฏิบัติตามขั้นตอนใดขั้นตอนหนึ่งต่อไปนี้
   - ในศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 ที่ ให้ไปที่ <https://compliance.microsoft.com>  \> **ตรวจสอบโซลูชัน** หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://compliance.microsoft.com/auditlogsearch> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderของ <https://security.microsoft.com> ที่ **ให้ไปที่** ตรวจสอบ หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://sip.security.microsoft.com/auditlogsearch> โดยตรง ให้ใช้

2. บนหน้า **ตรวจสอบ** ให้ตรวจสอบว่าเลือก **แท็บ** ค้นหา แล้วกําหนดค่าการตั้งค่าต่อไปนี้:
   - เลือกช่วงวันที่/เวลา **ในกล่อง** เริ่มต้น **และ** สิ้นสุด
   - ตรวจสอบว่า **กล่อง กิจกรรม** มี **แสดงผลลัพธ์กิจกรรมทั้งหมด**

3. เมื่อคุณเสร็จสิ้น **ให้คลิก** ค้นหา กิจกรรมจะปรากฏในหน้า **การค้นหาการตรวจสอบ** ใหม่

4. ในผลลัพธ์ ให้คลิก **กรองผลลัพธ์** แล้วพิมพ์ **Set-Mailbox** ในกล่องตัวกรองกิจกรรม

5. เลือกระเบียนการตรวจสอบในผลลัพธ์ ใน **ฟลาย** เอาท์ รายละเอียด **ให้คลิก** ข้อมูลเพิ่มเติม คุณต้องดูรายละเอียดของระเบียนการตรวจสอบแต่ละระเบียนเพื่อระบุว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมลหรือไม่

   - **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน
   - **พารามิเตอร์**: _ForwardingSmtpAddress_ จะระบุที่อยู่อีเมลเป้าหมาย
   - **UserId:** ผู้ใช้ที่กําหนดค่าการส่งต่ออีเมลบนกล่องจดหมายใน **เขตข้อมูล ObjectId**

For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
