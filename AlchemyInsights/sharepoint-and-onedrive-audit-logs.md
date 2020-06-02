---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509619"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>บันทึกการตรวจสอบของ SharePoint และ OneDrive

## <a name="sharepoint-classic-audit-logs"></a>บันทึกการตรวจสอบแบบคลาสสิคของ SharePoint

การตรวจสอบแบบดั้งเดิมของ SPO ถูกโยกย้ายไปบันทึกการตรวจสอบโดยรวม (UAL) รายงานการตรวจสอบ SPO แบบดั้งเดิมทั้งหมดจะได้รับพลังงานผ่าน UAL และสัญญาณการตรวจสอบแบบดั้งเดิมได้ถูกย้ายไปยัง UAL

การเปลี่ยนแปลงที่สําคัญ:

* การตัดแต่งไม่สามารถใช้ได้เป็นความสามารถ
* การเลือกเหตุการณ์เฉพาะเพื่อตรวจสอบจะไม่พร้อมใช้งาน อ้างอิง[ถึงเอกสารนี้](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)สําหรับรายการเหตุการณ์ที่ตรวจสอบทั้งหมดที่มีให้เป็นค่าเริ่มต้น
* ตัวเลือก**ตําแหน่งที่ตั้ง**ภายใต้**รายงานที่กําหนดเอง**ไม่พร้อมใช้งาน
* ตัวเลือก**การเปิดหรือการดาวน์โหลดเหตุการณ์เอกสาร**ไม่พร้อมใช้งาน

[การกําหนดค่าการตั้งค่าการตรวจสอบสําหรับไซต์คอลเลกชัน](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>บันทึกการตรวจสอบโดยรวมแบบสมัยใหม่ของ SharePoint และ OneDrive จากการปฏิบัติตามข้อกําหนด

* [เปิด/ปิดการบันทึกการตรวจสอบโดยรวม](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นภายใน SharePoint หรือ OneDrive

ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์โฟลเดอร์ผู้ใช้สิทธิ์:

* [กิจกรรมไฟล์และเพจ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [กิจกรรมโฟลเดอร์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [การแชร์และการเข้าถึงกิจกรรมคําขอ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [กิจกรรมการซิงโครไนส์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [กิจกรรมการดูแลไซต์](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกเหตุการณ์เหล่านี้ ให้ดูที่[การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
