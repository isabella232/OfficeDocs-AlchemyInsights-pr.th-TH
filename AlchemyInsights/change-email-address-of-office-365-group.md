---
title: เปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365อีเมล
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930748"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>เปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365อีเมล

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365ได้โดยใช้ศูนย์การจัดการ เพียงเลือกกลุ่ม @editที่อยู่อีเมลของคุณ

คุณยังสามารถใช้ตามสั่ง EXO PowerShell เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่มMicrosoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

ตัวอย่าง:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
