---
title: ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032577"
---
# <a name="control-access-to-public-folders-using-outlook"></a>ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้Outlook

เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะOutlookหนึ่งต่อไปนี้

1. ใช้ `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะOutlook  
$false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะOutlookโฟลเดอร์ นี่เป็นค่าเริ่มต้น  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

หมายเหตุ: กระบวนงานนี้สามารถควบคุมการเชื่อมต่อด้วยOutlookเดสก์ท็อปของคุณWindowsไคลเอ็นต์เท่านั้น ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะโดยใช้ OWA หรือOutlook for Macได้

For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.
