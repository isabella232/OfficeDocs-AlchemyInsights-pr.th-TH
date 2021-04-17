---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819099"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams โดยใช้ศูนย์การจัดการ[Microsoft 365](https://admin.microsoft.com/) เพียงเลือกกลุ่ม @editที่อยู่อีเมลของคุณ

คุณยังสามารถใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

ตัวอย่าง:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
