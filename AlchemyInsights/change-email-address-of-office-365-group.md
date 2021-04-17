---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819063"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 ได้โดยใช้ศูนย์การจัดการ เพียงเลือกกลุ่ม @editที่อยู่อีเมลของคุณ

คุณยังสามารถใช้ตามสั่ง EXO PowerShell เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

ตัวอย่าง:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
