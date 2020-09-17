---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812566"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะได้

ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทำงานสำหรับผู้ใช้บางรายให้ลองทำดังต่อไปนี้:

เชื่อมต่อกับ EXO PowerShell และกำหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox บนบัญชีผู้ใช้ที่มีปัญหาให้ตรงกับพารามิเตอร์บนบัญชีผู้ใช้ที่ทำงาน

ตัวอย่าง

WorkingUser การรับกล่องจดหมาย | ฟุต DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

การตั้งค่ากล่องจดหมาย ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล

ถ้าปัญหายังคงอยู่โปรดทำตาม [ขั้นตอน](https://aka.ms/pfcte) ต่อไปนี้เพื่อแก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
 
**เมื่อต้องการควบคุมผู้ใช้ที่สามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ทำ**ดังนี้

1.  ใช้การตั้งค่า-Set-casmailbox cmdlethttps <mailboxname> -PublicFolderClientAccess $true หรือ $false  
      
    $true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook  
      
    $false: ป้องกันไม่ให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook นี่เป็นค่าเริ่มต้น  
        
2.  ตั้งค่า-ชื่อ get-organizationconfig-PublicFolderShowClientControl $true   
      
**หมายเหตุ:** กระบวนงานนี้สามารถควบคุมการเชื่อมต่อได้เฉพาะกับไคลเอ็นต์ Outlook บนเดสก์ท็อปสำหรับ Windows เท่านั้น ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะได้อย่างต่อเนื่องโดยใช้ OWA หรือ Outlook for Mac
 
สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ประกาศการสนับสนุนสำหรับการควบคุมการเชื่อมต่อไปยังโฟลเดอร์สาธารณะใน Outlook](https://aka.ms/controlpf)