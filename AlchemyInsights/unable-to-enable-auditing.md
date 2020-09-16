---
title: ๒๔๑๙-ไม่สามารถเปิดใช้งาน-การตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767618"
---
# <a name="unable-to-enable-unified-auditing"></a>ไม่สามารถเปิดใช้งานการตรวจสอบแบบรวมได้

เมื่อคุณพยายามเปิดใช้งานการตรวจสอบแบบรวมสำหรับองค์กรของคุณคุณอาจได้รับข้อผิดพลาดคล้ายกับต่อไปนี้:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:

1. [เชื่อมต่อกับ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. เรียกใช้ cmdlet ต่อไปนี้:

   ```
   Enable-OrganizationCustomization
   ```

3. รอ๖๐นาทีสำหรับการตั้งค่าก่อนหน้านี้จะมีผล

4. เรียกใช้คำสั่งต่อไปนี้ใน Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

สำหรับข้อมูลเพิ่มเติมให้ดูบทความต่อไปนี้:

- [เชื่อมต่อกับ Exchange Online PowerShell โดยใช้การรับรองความถูกต้องแบบหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [เปิดหรือปิดการค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
