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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996649"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlookไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะ

ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ใช้งานได้กับผู้ใช้บางราย ให้ลองวิธีต่อไปนี้

เชื่อมต่อ EXO PowerShell และกําหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox บนบัญชีผู้ใช้ที่มีปัญหาให้ตรงกับพารามิเตอร์บนบัญชีผู้ใช้ที่ใช้งานได้

ตัวอย่าง:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command>

รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล

ถ้าปัญหายังคงอยู่ โปรดปฏิบัติตาม[กระบวนงานนี้](https://aka.ms/pfcte)เพื่อแก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้Outlook
 
**เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะOutlook:**

1.  ใช้ Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true หรือ $false  
      
    $true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะOutlook  
      
    $false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะOutlookโฟลเดอร์ นี่เป็นค่าเริ่มต้น  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**หมายเหตุ** กระบวนงานนี้สามารถควบคุมการเชื่อมต่อได้เฉพาะกับOutlookเดสก์ท็อปของคุณWindowsไคลเอ็นต์ของคุณ ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะโดยใช้ OWA หรือOutlook for Macได้
 
For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).