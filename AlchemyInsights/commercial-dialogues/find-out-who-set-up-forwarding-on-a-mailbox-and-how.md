---
title: ค้นหาว่าใครตั้งค่าการส่งต่อบนกล่องจดหมาย และวิธีการ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317827"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>ค้นหาว่าใครตั้งค่าการส่งต่อบนกล่องจดหมาย และวิธีการ

ถ้าตั้งค่าการส่งต่อภายนอกบนกล่องจดหมาย กิจกรรมจะถูกตรวจสอบเป็นส่วนหนึ่งของ cmdlet **ตั้งค่า** กล่องจดหมาย ต่อไปนี้เป็นวิธีการค้นหากิจกรรมในบันทึกการตรวจสอบ:

1. เลือกเลือกอย่างใดอย่างหนึ่งต่อไปนี้
   - ในศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 ที่ ให้ไปที่ <https://compliance.microsoft.com>  \> **ตรวจสอบโซลูชัน** หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://compliance.microsoft.com/auditlogsearch> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderของ <https://security.microsoft.com> ที่ **ให้ไปที่** ตรวจสอบ หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://security.microsoft.com/auditlogsearch> โดยตรง ให้ใช้

   **หมายเหตุ**: ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดการตรวจสอบ ให้เดินหน้าแล้วเปิดในตอนนี้ ถ้าไม่ได้เปิดฟีเจอร์นี้ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้

2. บนหน้า **ตรวจสอบ** ให้ตรวจสอบว่าเลือก **แท็บ** ค้นหา แล้วกําหนดค่าการตั้งค่าต่อไปนี้:
   - เลือกช่วงวันที่/เวลา **ในกล่อง** เริ่มต้น **และ** สิ้นสุด
   - ตรวจสอบว่า **กล่อง กิจกรรม** มี **แสดงผลลัพธ์กิจกรรมทั้งหมด**

3. เมื่อคุณเสร็จสิ้น **ให้คลิก** ค้นหา กิจกรรมจะปรากฏในหน้า **การค้นหาการตรวจสอบ** ใหม่

4. ในผลลัพธ์ ให้คลิกคอลัมน์ **กิจกรรม** เพื่อจัดเรียงผลลัพธ์ และมองหา **รายการ** ตั้งค่ากล่องจดหมาย

5. เลือกกิจกรรมในผลลัพธ์เพื่อเปิดเมนูปลิวรายละเอียด คุณต้องดูรายละเอียดของระเบียนการตรวจสอบแต่ละระเบียนเพื่อตรวจสอบว่ากิจกรรมเกี่ยวข้องกับการส่งต่ออีเมล:
   - **ObjectId**: ค่านามแฝงของกล่องจดหมายที่ถูกปรับเปลี่ยน
   - **พารามิเตอร์**: _ForwardingSmtpAddress_ จะระบุที่อยู่อีเมลเป้าหมาย
   - **UserId:** ผู้ใช้ที่กําหนดค่าการส่งต่ออีเมลบนกล่องจดหมายใน **เขตข้อมูล ObjectId**

For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
