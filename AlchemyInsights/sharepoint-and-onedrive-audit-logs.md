---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662227"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>บันทึกการตรวจสอบของ SharePoint และ OneDrive

## <a name="sharepoint-classic-audit-logs"></a>บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint

SPO การตรวจสอบดั้งเดิมถูกโยกย้ายไปยังบันทึกการตรวจสอบแบบรวม (UAL) ในตอนนี้รายงานการตรวจสอบแบบดั้งเดิมของ SPO ทั้งหมดจะได้รับการดำเนินการผ่าน UAL และจะมีการโยกย้ายสัญญาณการตรวจสอบแบบดั้งเดิมไปยัง UAL

การเปลี่ยนแปลงที่สำคัญ:

* การตัดแต่งจะไม่พร้อมใช้งานเป็นความสามารถ
* การเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบไม่พร้อมใช้งาน อ้างอิงไปยัง [เอกสารนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) สำหรับรายการของเหตุการณ์ที่ตรวจสอบทั้งหมดที่พร้อมใช้งานตามค่าเริ่มต้น
* ตัวเลือก **ตำแหน่งที่ตั้ง** ภายใต้ **รายงานแบบกำหนดเอง** จะไม่พร้อมใช้งาน
* ตัวเลือกการ **เปิดหรือการดาวน์โหลดเอกสาร** ไม่พร้อมใช้งาน

[การกำหนดค่าการตั้งค่าการตรวจสอบสำหรับไซต์คอลเลกชัน](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>บันทึกการตรวจสอบแบบครบวงจรของ SharePoint และ OneDrive จากการปฏิบัติตามกฎระเบียบ

* [เปิด/ปิดการบันทึกการตรวจสอบแบบครบวงจร](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive

ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์ (s), สิทธิ์การใช้งาน:

* [กิจกรรมของไฟล์และหน้า](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [กิจกรรมของโฟลเดอร์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [การแชร์และการร้องขอการเข้าถึงกิจกรรม](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [กิจกรรมการซิงโครไนซ์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [กิจกรรมการดูแลไซต์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกใช้เหตุการณ์เหล่านี้ให้ดู[ที่ค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
