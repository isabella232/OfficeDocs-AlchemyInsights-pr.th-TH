---
title: 2419-ไม่สามารถเปิดใช้งานการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510447"
---
# <a name="unable-to-enable-unified-auditing"></a>ไม่สามารถเปิดใช้งานการตรวจสอบแบบรวม

เมื่อคุณพยายามเปิดใช้งานการตรวจสอบแบบรวมสําหรับองค์กรของคุณ คุณอาจได้รับข้อผิดพลาดคล้ายคลึงกันต่อไปนี้:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:

1. [เชื่อมต่อกับ Powershell แบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. เรียกใช้ cmdlet ต่อไปนี้:

   ```
   Enable-OrganizationCustomization
   ```

3. รอ 60 นาทีเพื่อให้การตั้งค่าก่อนหน้านี้มีผล

4. เรียกใช้คําสั่งต่อไปนี้ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

สําหรับข้อมูลเพิ่มเติม ให้ดูบทความต่อไปนี้:

- [เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [เปิดหรือปิดการค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
