---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819531"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะ

ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ใช้งานได้กับผู้ใช้บางราย ให้ลองวิธีต่อไปนี้

เชื่อมต่อกับ EXO PowerShell และกําหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox บนบัญชีผู้ใช้ที่มีปัญหาให้ตรงกับพารามิเตอร์บนบัญชีผู้ใช้ที่ใช้งานได้

ตัวอย่าง:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command>

รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล

ถ้าปัญหายังคงอยู่ โปรดปฏิบัติตาม [กระบวนงานนี้](https://aka.ms/pfcte) เพื่อแก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
 
**เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook:**

1.  ใช้ Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true หรือ $false  
      
    $true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook  
      
    $false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook นี่เป็นค่าเริ่มต้น  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**หมายเหตุ** กระบวนงานนี้สามารถควบคุมการเชื่อมต่อด้วย Outlook บนเดสก์ท็อปไคลเอ็นต์ Windows เท่านั้น ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะต่อไปได้โดยใช้ OWA หรือ Outlook for Mac
 
For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).