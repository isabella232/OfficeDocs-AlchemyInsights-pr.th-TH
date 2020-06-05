---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580676"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 โดยใช้ศูนย์การจัดการ เพียงเลือกกลุ่มและเลือกที่อยู่อีเมล@edit

คุณยังสามารถใช้คําสั่งต่อไปนี้คําสั่ง EXO PowerShell เพื่อเปลี่ยนอยู่ SMTP หลักของกลุ่ม Microsoft 365:

ชุดรวมกลุ่ม <Group Name> -หลักSmtpที่อยู่<new SMTP Address>

ตัว อย่าง เช่น:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
