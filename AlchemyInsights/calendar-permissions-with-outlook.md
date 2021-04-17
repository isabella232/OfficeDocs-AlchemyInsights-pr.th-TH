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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819927"
---
# <a name="calendar-permissions"></a>สิทธิ์ในปฏิทิน

ผู้ใช้สามารถเปลี่ยนสิทธิ์ในปฏิทินของตนเองด้วย Outlook บนเว็บหรือไคลเอ็นต์อื่นๆ แต่ในฐานะผู้ดูแลระบบ คุณอาจต้องตรวจสอบด้วย  
ด้วย cmdlet ของ Exchange PowerShell จะแสดงสิทธิ์บนปฏิทินของผู้ใช้:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

เมื่อต้องการดูข้อมูลเพิ่มเติม ให้ดูรายการต่อไปนี้

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

สิทธิ์ในปฏิทินจะใช้ในการแชร์ปฏิทิน เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการแชร์ปฏิทิน Outlook ให้ดูบทความเหล่านี้:

- [แชร์ปฏิทิน Outlook กับบุคคลอื่น](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [แชร์ปฏิทินใน Outlook บนเว็บ for Business](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

เมื่อต้องการแก้ไขปัญหาสิทธิ์ในปฏิทิน คุณสามารถใช้ [เครื่องมือตัวช่วยการสนับสนุนและ](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) การกู้คืนได้