---
title: รายงานบันทึกการตรวจสอบของ SharePoint แบบคลาสสิก
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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741984"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>บันทึกการตรวจสอบ SharePoint และ OneDrive

## <a name="sharepoint-classic-audit-logs"></a>บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint

การตรวจสอบแบบดั้งเดิมของ SPO ถูกโยกย้ายไปยังบันทึกการตรวจสอบรวม (UAL) รายงานการตรวจสอบแบบดั้งเดิมของ SPO ทั้งหมดจะถูกขับเคลื่อนผ่าน UAL และสัญญาณการตรวจสอบแบบดั้งเดิมได้ถูกย้ายไปยัง UAL

การเปลี่ยนแปลงที่สําคัญ:

* การตัดแต่งไม่พร้อมใช้งานเป็นความสามารถ
* การเลือกเหตุการณ์เฉพาะที่จะตรวจสอบไม่พร้อมใช้งาน โปรดดู[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สําหรับรายการเหตุการณ์ที่ตรวจสอบทั้งหมดที่พร้อมใช้งานตามค่าเริ่มต้น
* ตัวเลือก**ตําแหน่ง**ภายใต้**รายงานที่กําหนดเอง**จะไม่พร้อมใช้งาน
* ตัวเลือก**การเปิดหรือดาวน์โหลด**เอกสารเหตุการณ์ไม่สามารถใช้ได้

[การกําหนดค่าการตรวจสอบการตั้งค่าสําหรับไซต์คอลเลกชัน](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>บันทึกการตรวจสอบแบบครบวงจรสมัยใหม่ของ SharePoint และ OneDrive จากการปฏิบัติตามกฎระเบียบ

* [เปิด/ปิดการบันทึกการตรวจสอบรวม](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

ไม่มีการกําหนดค่าเพิ่มเติมที่จําเป็นภายใน SharePoint หรือ OneDrive

ใช้การค้นหาการบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของแฟ้ม, โฟลเดอร์, user(s),

* [กิจกรรมไฟล์และเพจ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [กิจกรรมโฟลเดอร์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [กิจกรรมการแชร์และการร้องขอการเข้าถึง](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [กิจกรรมการซิงโครไนส์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [กิจกรรมการดูแลไซต์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกเหตุการณ์เหล่านี้ ให้ดูที่[การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
