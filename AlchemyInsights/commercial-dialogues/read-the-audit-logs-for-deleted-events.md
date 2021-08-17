---
title: อ่านบันทึกการตรวจสอบของเหตุการณ์ที่ถูกลบ
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896034"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>อ่านบันทึกการตรวจสอบของเหตุการณ์ที่ถูกลบ

วิธีการมีดังนี้

1. เลือกเลือกอย่างใดอย่างหนึ่งต่อไปนี้
   - ในศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 ที่ ให้ไปที่ <https://compliance.microsoft.com>  \> **ตรวจสอบโซลูชัน** หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://compliance.microsoft.com/auditlogsearch> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderที่ <https://security.microsoft.com> **ให้ไปที่** ตรวจสอบ หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://security.microsoft.com/auditlogsearch> โดยตรง ให้ใช้

    > [!NOTE]
    > ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดฟีเจอร์นี้ ให้เปิดใช้งานทันที ถ้าฟีเจอร์ไม่ได้เปิดใช้งาน ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้

2. บนแท็บ **ค้นหา** ของหน้า **ตรวจสอบ** ให้กําหนดค่าการตั้งค่าต่อไปนี้
   - **ช่วงวันที่และเวลา**: เลือกช่วงวันที่/เวลา **ในกล่อง** เริ่มต้น **และ** สิ้นสุด
   - **กิจกรรม**: **Exchangeกิจกรรมกล่องจดหมาย** ของคุณ แล้วเลือกค่าต่อไปนี้:
     - **ข้อความที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ**
     - **ย้ายข้อความไปยังโฟลเดอร์รายการที่ถูกลบแล้ว**

       เมื่อคุณเสร็จสิ้น ให้คลิกภายนอกบานหน้าต่างเพื่อย่อ **บานหน้าต่าง กิจกรรม**

   - **ผู้ใช้**: ยอมรับค่าเริ่มต้นว่างเพื่อส่งกลับผลลัพธ์ของผู้ใช้ทั้งหมด หรือใส่ผู้ใช้อย่างน้อยหนึ่งราย

3. เมื่อคุณเสร็จสิ้น **ให้คลิก** ค้นหา กิจกรรมจะปรากฏในหน้า **การค้นหาการตรวจสอบ** ใหม่

4. เลือกกิจกรรมในผลลัพธ์เพื่อเปิดเมนูปลิวรายละเอียด ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ เช่น บรรทัดเรื่องและที่ตั้งของรายการเมื่อรายการถูกลบ จะแสดงอยู่ใน **เขตข้อมูล AffectedItems**

   > [!NOTE]
   > คุณไม่สามารถคืนค่ารายการที่ถูกลบโดยใช้ฟีเจอร์บันทึกการตรวจสอบได้ เมื่อต้องการคืนค่ารายการที่ถูกลบ[ให้ดู กู้คืนข้อความอีเมลที่ถูกลบใน Outlook บนเว็บ](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

For more information, see [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
