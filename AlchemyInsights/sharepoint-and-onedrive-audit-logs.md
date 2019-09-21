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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068042"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>บันทึกการตรวจสอบ SharePoint และ OneDrive

**SharePoint และ OneDrive ทันสมัยรวมบันทึกการตรวจสอบจากการปฏิบัติตามกฎระเบียบ**

- [เปิด/ปิดการบันทึกการตรวจสอบรวม](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

ไม่จำเป็นต้องมีการกำหนดค่าเพิ่มเติมภายใน SharePoint หรือ OneDrive

- ใช้การค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบกิจกรรมของไฟล์ (s), โฟลเดอร์, ผู้ใช้ (s), สิทธิ์:

    - [กิจกรรมของแฟ้มและเพจ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [กิจกรรมโฟลเดอร์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [การแชร์และการเข้าถึงกิจกรรมการร้องขอ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [กิจกรรมการซิงโครไนส์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [กิจกรรมการดูแลไซต์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการค้นคืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)

**บันทึกการตรวจสอบแบบคลาสสิกของ SharePoint**

เราย้ายการตรวจสอบที่สืบทอดมาจากการตรวจสอบรวม นี่เป็นหลักหมายความว่ารายงานการตรวจสอบแบบดั้งเดิมของทั้งหมดของทั้งหมดจะถูกขับเคลื่อนผ่านด้านหน้าและมีการโยกย้ายสัญญาณการตรวจสอบเดิม

การเปลี่ยนแปลงที่สำคัญ:

- การตัดแต่งเป็นความสามารถไม่พร้อมใช้งาน
- ส่วนที่คุณเลือกเหตุการณ์ที่เฉพาะเจาะจงในการตรวจสอบจะไม่พร้อมใช้งาน โปรดดูที่[เอกสารนี้](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)สำหรับรายการทั้งหมดของเหตุการณ์ที่ตรวจสอบพร้อมใช้งานตามค่าเริ่มต้น
- ตัวเลือก "ตำแหน่ง" ภายใต้**รายงานที่กำหนดเอง**ไม่พร้อมใช้งาน 
- เหตุการณ์ "การเปิดหรือดาวน์โหลดเอกสาร" ไม่พร้อมใช้งาน 

