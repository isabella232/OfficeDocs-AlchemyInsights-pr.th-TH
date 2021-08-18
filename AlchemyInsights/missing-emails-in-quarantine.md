---
title: อีเมลหายไปในการกักกัน
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
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329681"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลหายไปในการกักกัน

ผู้ดูแลระบบสามารถดู [เผยแพร่ หรือลบข้อความเหล่านี้ได้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

ในMicrosoft 365 Defenderที่ <https://security.microsoft.com> ไปที่ **ตรวจทาน** \> **การกัก** กัน หรือเมื่อต้องการไปที่หน้า **การกัก** กัน โดยตรง <https://security.microsoft.com/quarantine> ให้ใช้  

For more information about the search/filter values that you can use, see [Manage quarantined messages and files as an admin in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

cmdlet ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในการกักกันคือ:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [การกักกันแสดงตัวอย่าง :](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้จะมีไว้เฉพาะข้อความเท่านั้น ไม่ใช่ไฟล์จากตู้เซฟสิ่งที่แนบมาSharePoint OneDrive หรือ Microsoft Teams
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
