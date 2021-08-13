---
title: 2419-ไม่สามารถเปิดใช้งานการตรวจสอบได้
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007809"
---
# <a name="unable-to-enable-unified-auditing"></a>ไม่สามารถเปิดใช้งานการตรวจสอบแบบรวม

เมื่อคุณพยายามเปิดใช้งานการตรวจสอบแบบรวมขององค์กรของคุณ คุณอาจได้รับข้อผิดพลาดที่คล้ายกันต่อไปนี้:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. [เชื่อมต่อ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. เรียกใช้ cmdlet ต่อไปนี้:

   ```
   Enable-OrganizationCustomization
   ```

3. รอ 60 นาทีเพื่อให้การตั้งค่าก่อนหน้ามีผล

4. เรียกใช้สั่งต่อไปนี้ใน Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

ดูบทความต่อไปนี้เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับข้อมูลเพิ่มเติม:

- [เชื่อมต่อ powershell Exchange Online โดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [เปิดหรือปิดการค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
