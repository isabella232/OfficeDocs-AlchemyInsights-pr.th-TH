---
title: การควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804004"
---
# <a name="control-access-to-public-folders-using-outlook"></a>การควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook

เมื่อต้องการควบคุมผู้ใช้ที่สามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ทำดังนี้

1. ใช้ `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook  
$false: ป้องกันไม่ให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook นี่เป็นค่าเริ่มต้น  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

หมายเหตุ: กระบวนการนี้สามารถควบคุมการเชื่อมต่อกับไคลเอ็นต์ Outlook บนเดสก์ท็อปสำหรับ Windows ได้เท่านั้น ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะได้ต่อไปโดยใช้ OWA หรือ Outlook for Mac

สำหรับข้อมูลเพิ่มเติมให้ดู [ที่การควบคุมการเชื่อมต่อไปยังโฟลเดอร์สาธารณะใน Outlook](https://aka.ms/controlpf) สำหรับข้อมูลเพิ่มเติม
