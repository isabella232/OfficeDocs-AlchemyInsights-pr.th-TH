---
title: รายงานบันทึกการตรวจสอบ SharePoint แบบคลาสสิก
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992637"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>บันทึกการตรวจสอบ SharePoint และ OneDrive

## <a name="sharepoint-classic-audit-logs"></a>บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint

การตรวจสอบดั้งเดิมของที่ได้รับการโยกย้ายไปยังบันทึกการตรวจสอบรวม (นวล) ขณะนี้รายงานการตรวจสอบแบบดั้งเดิมของที่ได้รับการสนับสนุนทั้งหมดจะถูกใช้งานผ่านทางด้านหน้าและมีการย้ายสัญญาณการตรวจสอบแบบดั้งเดิมไปยัง

การเปลี่ยนแปลงที่สำคัญ:

* การตัดแต่งไม่สามารถใช้ได้เป็นความสามารถ
* การเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบไม่สามารถใช้ได้ อ้างอิงถึง[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สำหรับรายการที่สมบูรณ์ของเหตุการณ์ที่ตรวจสอบพร้อมใช้งานตามค่าเริ่มต้น
* ตัวเลือกที่**ตั้ง**ภายใต้**รายงานที่กำหนดเอง**ไม่พร้อมใช้งาน
* ตัวเลือกการ**เปิดหรือดาวน์โหลดเอกสาร**เหตุการณ์ไม่พร้อมใช้งาน

[กำหนดการตั้งค่าการตรวจสอบสำหรับชุดเก็บรวบรวมไซต์](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint และ OneDrive ทันสมัยรวมบันทึกการตรวจสอบจากการปฏิบัติตามกฎระเบียบ

* [เปิด/ปิดการบันทึกการตรวจสอบรวม](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive

ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์, ผู้ใช้ (s), สิทธิ์:

* [กิจกรรมของแฟ้มและเพจ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [กิจกรรมโฟลเดอร์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [การแชร์และการเข้าถึงกิจกรรมการร้องขอ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [กิจกรรมการซิงโครไนส์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [กิจกรรมการดูแลไซต์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการค้นคืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
