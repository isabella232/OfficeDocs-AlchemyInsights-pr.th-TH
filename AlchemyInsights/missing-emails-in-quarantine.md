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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892066"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลหายไปในการกักกัน

ผู้ดูแลระบบสามารถดู [เผยแพร่ หรือลบข้อความเหล่านี้ได้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

ในMicrosoft 365 Defenderที่ <https://security.microsoft.com> ให้ไปที่ **ตรวจทาน** \> **การกัก** กัน หรือเมื่อต้องการไปที่หน้า **การกัก** กัน โดยตรง <https://security.microsoft.com/quarantine> ให้ใช้  

For more information about the search/filter values that you can use, see [Manage quarantined messages and files as an admin in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

cmdlet ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในการกักกันคือ:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [การกักกันแสดงตัวอย่าง :](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้จะมีไว้เฉพาะข้อความเท่านั้น ไม่ใช่ไฟล์จากตู้เซฟสิ่งที่แนบมาSharePoint OneDrive หรือ Microsoft Teams
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
