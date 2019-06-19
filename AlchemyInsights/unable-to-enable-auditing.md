---
title: 2419-ไม่การเปิดใช้งานการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065717"
---
# <a name="unable-to-enable-unified-auditing"></a>ไม่สามารถเปิดใช้งานการตรวจสอบประกอบการ

เมื่อคุณพยายามที่จะเปิดใช้งานการตรวจสอบสำหรับองค์กรของคุณ Office 365 ประกอบการ คุณอาจได้รับข้อผิดพลาดที่คล้ายคลึงกันต่อไปนี้:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:

1. การ[เชื่อมต่อการแลกเปลี่ยน Powershell แบบออนไลน์](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. เรียกใช้ cmdlet ต่อไปนี้:

   ```
   Enable-OrganizationCustomization
   ```

3. รอ 60 นาทีสำหรับการตั้งค่าก่อนหน้านี้มีผลบังคับใช้

4. เรียกใช้คำสั่งต่อไปนี้ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

สำหรับข้อมูลเพิ่มเติม ดูบทความต่อไปนี้:

- [เชื่อมต่อกับ Exchange PowerShell แบบออนไลน์โดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [เปิด หรือปิดการค้นหาแฟ้มบันทึกการตรวจสอบ Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
