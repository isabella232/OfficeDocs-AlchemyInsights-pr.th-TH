---
title: ระบุกิจกรรมกฎสำหรับกล่องจดหมายเข้าในบันทึกการตรวจสอบ
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779070"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>ระบุกิจกรรมกฎสำหรับกล่องจดหมายเข้าในบันทึกการตรวจสอบ

คุณสามารถใช้การค้นหาบันทึกการตรวจสอบในศูนย์การรักษาความปลอดภัย & ของ Microsoft ๓๖๕เพื่อดูเหตุการณ์ของกฎสำหรับกล่องจดหมายเข้า (การสร้างการปรับเปลี่ยนและการลบกฎของกล่องจดหมายเข้า)

1. ลงชื่อเข้าใช้[ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)

2. ไปที่หน้า**Search**  >  **ค้นหาบันทึกการตรวจสอบ**การค้นหา

3. เลือกช่วงวันที่ในเขตข้อมูลวันที่**เริ่มต้น**และ**วันที่สิ้นสุด**

4. ภายใต้**กิจกรรมกล่องจดหมาย Exchange**ให้ตรวจสอบว่าเขตข้อมูล**กิจกรรม**ถูกตั้งค่าเป็น**InboxRule สร้าง/แก้ไข/เปิดใช้งานกฎกล่องจดหมายเข้าใหม่**

5. คลิก**ค้นหา**

ในผลลัพธ์ให้เลือกระเบียนการตรวจสอบ ในเมนูรายละเอียดให้คลิก**ข้อมูลเพิ่มเติม** ข้อมูลเกี่ยวกับการตั้งค่ากฎสำหรับกล่องจดหมายเข้าจะแสดงอยู่ในเขตข้อมูล**พารามิเตอร์**

สำหรับข้อมูลเพิ่มเติมให้ดูที่[การกำหนดว่าผู้ใช้สร้างกฎกล่องจดหมายเข้าหรือ](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)ไม่
