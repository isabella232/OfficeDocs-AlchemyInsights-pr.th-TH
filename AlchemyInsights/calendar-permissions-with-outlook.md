---
title: สิทธิ์ในปฏิทิน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046123"
---
# <a name="calendar-permissions"></a>สิทธิ์ในปฏิทิน

ผู้ใช้สามารถเปลี่ยนสิทธิ์ในปฏิทินของตนเองOutlookปฏิทินบนเว็บหรือไคลเอ็นต์อื่นๆ ได้ แต่ในฐานะผู้ดูแลระบบ คุณอาจต้องตรวจสอบด้วย  
With Exchange PowerShell cmdlet will show you the permission on a user's calendar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

เมื่อต้องการดูข้อมูลเพิ่มเติม ให้ดูรายการต่อไปนี้

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

สิทธิ์ในปฏิทินจะถูกใช้ในการแชร์ปฏิทิน เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการแชร์Outlookปฏิทินของคุณ ให้ดูบทความเหล่านี้:

- [แชร์Outlookปฏิทินกับบุคคลอื่น](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [แชร์ปฏิทินOutlook บนเว็บธุรกิจ](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

เมื่อต้องการแก้ไขปัญหาสิทธิ์ในปฏิทิน คุณสามารถใช้[ตัวช่วยการสนับสนุนและการกู้คืน](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)ปฏิทินได้