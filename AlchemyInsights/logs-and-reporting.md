---
title: แฟ้มบันทึกและการรายงาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067031"
---
# <a name="logs-and-reporting"></a>แฟ้มบันทึกและการรายงาน

[Azure Active Directoryตอบคําถาม](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq)ที่ถามบ่อยเกี่ยวกับAzure Active Directory (Azure AD) ดูข้อมูลเพิ่มเติมในรายงาน[Azure Active Directoryรายงาน](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)

**การแก้ไขปัญหาเกี่ยวกับการตรวจสอบ**

1. หากคุณมีปัญหาในการดูกิจกรรมการตรวจสอบบางอย่างและกิจกรรมที่หายไปอยู่ใน [รายการนี้](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)โปรดส่งตั๋วการสนับสนุน
2. ถ้าคุณมีปัญหาในการดูบันทึกการตรวจสอบใดๆ ในผู้เช่าของคุณ โปรดส่งตั๋วการสนับสนุน
3. ถ้ากิจกรรมการตรวจสอบของคุณไม่แสดงขึ้นทันทีในพอร์ทัล Azure ให้ตรวจสอบข้อมูลเวลาแฝงของเรา [และจัดเก็บ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงที่บันทึก
4. [การเก็บข้อมูลแฟ้มบันทึกกิจกรรม Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. ถ้าคุณไม่เห็นการตรวจสอบทั้งหมดเกี่ยวกับช่วงวันที่ที่คุณเลือก คุณสามารถดาวน์โหลดแถวได้ถึง 250K (เรียงล.งจากล่าสุด) ของการเข้าสู่ระบบจากพอร์ทัล Azure หากต้องการข้อมูลเพิ่มเติม โปรดดู [ดาวน์โหลดกิจกรรม](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)การตรวจสอบ

**การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้**

1. คุณสามารถดูข้อมูลได้เพียง 30 วันที่ผ่านมาถ้าคุณมีสิทธิ์การใช้งาน Azure AD Premium (P1 หรือ P2) ของผู้เช่าของคุณ
2. การลงชื่อเข้าใช้จะพร้อมใช้งานเฉพาะกับผู้เช่า azure AD Premiumเท่านั้น ซึ่งไม่มีให้ใช้งานในผู้เช่าที่มีสิทธิ์การใช้งานแบบฟรีหรือแบบพื้นฐาน
3. ถ้าผู้เช่าของคุณมีสิทธิ์การใช้งาน Premium P1 และคุณไม่สามารถดูการลงชื่อเข้าใช้ ได้ ให้ตรวจสอบข้อมูลเวลาแฝงของเรา และ[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)ส่งตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงที่บันทึก
4. ถ้าคุณไม่เห็นการลงชื่อเข้าใช้ทั้งหมดในช่วงของวันที่ที่คุณเลือก โปรดทราบว่า คุณสามารถดาวน์โหลดแถวได้ถึง 250K (เรียงล.ยตามล่าสุด) ของการลงชื่อเข้าใช้จากพอร์ทัล Azure หากต้องการข้อมูลเพิ่มเติม โปรดดู [ดาวน์โหลดกิจกรรมการ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)ลงชื่อเข้าใช้

**แก้ไขปัญหารายงานความปลอดภัย (ผู้ใช้ที่ถูกตั้งค่าสถานะที่มีความเสี่ยง การลงชื่อเข้าใช้ที่มีความเสี่ยง)**

1. [ผู้ใช้ที่ถูกตั้งค่าสถานะเป็นรายงานด้านความปลอดภัยของความเสี่ยง](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [รายงานการลงชื่อเข้าใช้ที่มีความเสี่ยงในAzure Active Directoryการเข้าถึง](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directoryเหตุการณ์ความเสี่ยง](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
