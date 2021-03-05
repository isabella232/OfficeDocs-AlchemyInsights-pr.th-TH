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
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483417"
---
# <a name="auditing-in-microsoft-365"></a>การตรวจสอบใน Microsoft 365

ต่อไปนี้เป็นบางสิ่งที่คุณควรทราบเกี่ยวกับการตรวจสอบใน Microsoft 365:

1. กิจกรรมผู้ดูแลระบบ Exchange จะถูกตรวจสอบตามค่าเริ่มต้น
1. เราอยู่ในระหว่างการเปิดใช้งานการตรวจสอบกล่องจดหมายตามค่าเริ่มต้นของผู้ใช้ทั้งหมด เมื่อต้องการอ่านเพิ่มเติมเกี่ยวกับเรื่องนี้ [ให้คลิก](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)ที่นี่ จนกว่าจะถึงตอนนี้ ถ้าคุณต้องการคําแนะนําให้เปิดใช้งานด้วยตนเองให้กับบุคคลหนึ่งคนหรือทั้งองค์กร ให้เลือกปุ่มเปิดการตรวจสอบกล่องจดหมายด้านล่าง
1. กล่องจดหมายกลุ่ม Microsoft 365 และกล่องจดหมายโฟลเดอร์สาธารณะไม่สนับสนุนบันทึกการตรวจสอบ
1. For SharePoint/OneDrive, there is no additional configuration required to enabled auditing. เมื่อต้องการเรียนรู้ว่ากิจกรรมอะไรได้รับการตรวจสอบ ให้ดู:
    1. [กิจกรรมของไฟล์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [กิจกรรมของโฟลเดอร์](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [กิจกรรมการแชร์และ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)การเข้าถึง
1. ดูกิจกรรมผ่านการตรวจสอบทั้งหมดตามบริการ [เพื่อดูกิจกรรมที่ผ่าน](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)การตรวจสอบ
