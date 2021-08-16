---
title: การตรวจสอบใน Microsoft 365
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
ms.openlocfilehash: a5acd322186f8f4b7734f8541877a642a553288e10b3c122e4f276b9bb611308
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988998"
---
# <a name="auditing-in-microsoft-365"></a>การตรวจสอบใน Microsoft 365

ต่อไปนี้คือบางสิ่งที่คุณควรทราบเกี่ยวกับการตรวจสอบในMicrosoft 365:

1. Exchangeกิจกรรมผู้ดูแลระบบของคุณจะถูกตรวจสอบตามค่าเริ่มต้น
1. เราอยู่ในระหว่างการเปิดใช้งานการตรวจสอบกล่องจดหมายตามค่าเริ่มต้นของผู้ใช้ทั้งหมด เมื่อต้องการอ่านเพิ่มเติมเกี่ยวกับสิ่งนี้ [ให้คลิก](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)ที่นี่ ก่อนถึงเวลานั้น ถ้าคุณต้องการคําแนะนําในการเปิดใช้งานด้วยตนเองให้กับบุคคลหนึ่งคนหรือทั้งองค์กร ให้เลือกปุ่ม เปิดการตรวจสอบกล่องจดหมาย ที่ด้านล่าง
1. Microsoft 365 กล่องจดหมายกลุ่มและกล่องจดหมายโฟลเดอร์สาธารณะไม่สนับสนุนบันทึกการตรวจสอบ
1. For SharePoint/OneDrive, there is no additional configuration required to enabled auditing. เมื่อต้องการเรียนรู้ว่ากิจกรรมอะไรได้รับการตรวจสอบ ให้ดู:
    1. [กิจกรรมของไฟล์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [กิจกรรมของโฟลเดอร์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [กิจกรรมการแชร์และ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)การเข้าถึง
1. ดูรายการกิจกรรมตรวจสอบแล้วทั้งหมดตามบริการ[ให้ดู กิจกรรมการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)
