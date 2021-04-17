---
title: ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816759"
---
# <a name="control-access-to-public-folders-using-outlook"></a>ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook

เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ต่อไปนี้

1. ใช้ `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook  
$false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook นี่เป็นค่าเริ่มต้น  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

หมายเหตุ: กระบวนงานนี้สามารถควบคุมการเชื่อมต่อกับ Outlook บนเดสก์ท็อปของไคลเอ็นต์ Windows เท่านั้น ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะต่อไปได้โดยใช้ OWA หรือ Outlook for Mac

For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.
