---
title: ระบุกิจกรรมกฎกล่องจดหมายเข้าในบันทึกการตรวจสอบ
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891314"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>ระบุกิจกรรมกฎกล่องจดหมายเข้าในบันทึกการตรวจสอบ

คุณสามารถใช้การค้นหาบันทึกการตรวจสอบในมุมมองศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365เหตุการณ์กฎกล่องจดหมายเข้า (การสร้าง การปรับเปลี่ยน และลบกฎกล่องจดหมายเข้า)

1. ให้เลือกปฏิบัติตามขั้นตอนใดขั้นตอนหนึ่งต่อไปนี้
   - ในศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 ที่ ให้ไปที่ <https://compliance.microsoft.com>  \> **ตรวจสอบโซลูชัน** หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://compliance.microsoft.com/auditlogsearch> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderที่ <https://security.microsoft.com> **ให้ไปที่** ตรวจสอบ หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://security.microsoft.com/auditlogsearch> โดยตรง ให้ใช้

2. บนแท็บ **ค้นหา** ของหน้า **ตรวจสอบ** ให้กําหนดค่าการตั้งค่าต่อไปนี้
   - **ช่วงวันที่และเวลา**: เลือกช่วงวันที่/เวลา **ในกล่อง** เริ่มต้น **และ** สิ้นสุด
   - **กิจกรรม**: เลือกค่าอย่างน้อยหนึ่งค่าต่อไปนี้:
     - **กฎกล่องจดหมายเข้าใหม่ กฎการสร้างกล่องจดหมายเข้าOutlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **อัปเดตกฎกล่องจดหมายเข้าOutlookไคลเอ็นต์**

3. เมื่อคุณเสร็จสิ้น **ให้คลิก** ค้นหา กิจกรรมจะปรากฏในหน้า **การค้นหาการตรวจสอบ** ใหม่

4. เลือกกิจกรรมในผลลัพธ์เพื่อเปิดเมนูปลิวรายละเอียด ข้อมูลเกี่ยวกับการตั้งค่ากฎกล่องจดหมายเข้าจะแสดง **ในเขตข้อมูล** พารามิเตอร์

For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
