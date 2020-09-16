---
title: สิทธิ์ของปฏิทิน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748812"
---
# <a name="calendar-permissions"></a>สิทธิ์ของปฏิทิน

ผู้ใช้สามารถเปลี่ยนแปลงสิทธิ์ของปฏิทินของตนเองกับ Outlook บนเว็บหรือไคลเอ็นต์อื่นๆได้แต่เป็นผู้ดูแลระบบที่คุณอาจต้องการตรวจสอบด้วยเช่นกัน  
ด้วย cmdlet PowerShell Exchange จะแสดงสิทธิ์ในปฏิทินของผู้ใช้:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

เมื่อต้องการดูข้อมูลเพิ่มเติมให้ดูที่ข้อมูลต่อไปนี้:

- [รับ-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [ตั้งค่า-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

สิทธิ์ของปฏิทินจะถูกใช้ในการแชร์ปฏิทินเพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการแชร์ปฏิทิน Outlook ให้ดูบทความเหล่านี้:

- [แชร์ปฏิทิน Outlook กับบุคคลอื่น](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [แชร์ปฏิทินของคุณใน Outlook บนเว็บสำหรับธุรกิจ](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

เมื่อต้องการแก้ไขปัญหาสิทธิ์การใช้งานปฏิทินคุณสามารถใช้เครื่องมือการ[สนับสนุนและตัวช่วยการกู้คืน](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)