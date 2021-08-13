---
title: เปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365อีเมลMicrosoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995641"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>เปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365อีเมลMicrosoft Teams

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่มMicrosoft 365หรือMicrosoft Teams โดยใช้ศูนย์การจัดการ Microsoft 365 [](https://admin.microsoft.com/) เพียงเลือกกลุ่ม @editที่อยู่อีเมลของคุณ

คุณยังสามารถใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม/Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

ตัวอย่าง:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
