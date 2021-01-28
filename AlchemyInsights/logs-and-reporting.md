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
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036098"
---
# <a name="logs-and-reporting"></a>แฟ้มบันทึกและการรายงาน

[คําตอบที่ถามบ่อยเกี่ยวกับ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) การรายงาน Azure Active Directory (Azure AD) ของการรายงานของ Azure Active Directory For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**การแก้ไขปัญหาเกี่ยวกับการตรวจสอบ**

1. หากคุณมีปัญหาในการดูกิจกรรมการตรวจสอบบางอย่างและกิจกรรมที่หายไปอยู่ใน [รายการนี้](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)โปรดส่งตั๋วการสนับสนุน
2. ถ้าคุณมีปัญหาในการดูบันทึกการตรวจสอบใดๆ ในผู้เช่าของคุณ โปรดส่งตั๋วการสนับสนุน
3. ถ้ากิจกรรมการตรวจสอบของคุณไม่แสดงขึ้นทันทีในพอร์ทัล Azure ให้ตรวจสอบข้อมูลเวลาแฝงของเรา[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)และจัดเก็บตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงที่บันทึก
4. [การเก็บข้อมูลบันทึกกิจกรรม Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. ถ้าคุณไม่เห็นการตรวจสอบทั้งหมดในช่วงวันที่ที่คุณเลือก คุณสามารถดาวน์โหลดแถวได้มากถึง 250K (เรียงล>บตามล>นล่าสุด) ของการลงชื่อเข้าใช้จากพอร์ทัล Azure หากต้องการข้อมูลเพิ่มเติม โปรดดู[การดาวน์โหลดกิจกรรมการตรวจสอบ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)

**การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้**

1. คุณสามารถดูข้อมูลได้เพียง 30 วันสุดท้ายถ้าคุณมีสิทธิ์การใช้งาน Azure AD Premium (P1 หรือ P2) ของผู้เช่าของคุณ
2. การลงชื่อเข้าใช้จะพร้อมใช้งานเฉพาะกับผู้เช่า Azure AD Premium เท่านั้น ซึ่งไม่มีให้ใช้งานในผู้เช่าที่มีสิทธิ์การใช้งานแบบฟรีหรือแบบพื้นฐาน
3. ถ้าผู้เช่าของคุณมีสิทธิ์การใช้งาน P1 แบบพรีเมียม และคุณไม่สามารถดูการลงชื่อเข้าใช้ ให้ดูข้อมูลเวลาแฝงของเรา[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)และเปิดไฟล์ตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงของเอกสาร
4. ถ้าคุณไม่เห็นการลงชื่อเข้าใช้ทั้งหมดในช่วงวันที่ที่คุณเลือก โปรดสังเกตว่าคุณสามารถดาวน์โหลดแถวได้ถึง 250K (เรียงล>บตามล่าสุด) ของการลงชื่อเข้าใช้จากพอร์ทัล Azure หากต้องการข้อมูลเพิ่มเติม [โปรดดูการดาวน์โหลดกิจกรรมการ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)ลงชื่อเข้าใช้

**แก้ไขปัญหารายงานความปลอดภัย (ผู้ใช้ที่ถูกตั้งค่าสถานะที่มีความเสี่ยง การลงชื่อเข้าใช้ที่มีความเสี่ยง)**

1. [ผู้ใช้ที่ถูกตั้งค่าสถานะรายงานด้านความปลอดภัยของความเสี่ยง](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [รายงานการลงชื่อเข้าใช้ที่มีความเสี่ยงในพอร์ทัล Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [เหตุการณ์ความเสี่ยง Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
