---
title: เปลี่ยนที่อยู่อีเมลของ Microsoft ๓๖๕กลุ่มหรือทีม Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756576"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>เปลี่ยนที่อยู่อีเมลของ Microsoft ๓๖๕กลุ่มหรือทีม Microsoft

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕หรือทีม Microsoft ได้โดยใช้[ศูนย์การจัดการ Microsoft ๓๖๕](https://admin.microsoft.com/) เพียงเลือกกลุ่มแล้วเลือก @edit อีเมลแอดเดรส

คุณยังสามารถใช้คำสั่ง EXO PowerShell ต่อไปนี้เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม/ทีม Microsoft ๓๖๕:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

ตัวอย่าง

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
