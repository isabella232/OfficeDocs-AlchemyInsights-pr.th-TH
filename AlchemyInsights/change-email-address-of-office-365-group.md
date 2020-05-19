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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283263"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 โดยใช้ศูนย์การจัดการ เพียงเลือกกลุ่มและเลือกที่อยู่อีเมล@edit

คุณยังสามารถใช้ต่อไปนี้คําสั่ง PowerShell EXO เพื่อเปลี่ยนอยู่ SMTP หลักของกลุ่ม Microsoft 365:

ตั้งค่า-รวมกลุ่ม <Group Name> -หลักที่อยู่<new SMTP Address>

ตัว อย่าง เช่น:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
