---
title: ไม่สามารถเปลี่ยนชื่อผู้ใช้ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020247"
---
# <a name="unable-to-change-username"></a>ไม่สามารถเปลี่ยนชื่อผู้ใช้ได้

ในบางกรณี การเปลี่ยนแปลง UPN (UserPrincipalName) จะไม่เผยแพร่ไปยังระบบคลาวด์ คุณอาจได้รับข้อผิดพลาดการตรวจสอบความถูกต้องOffice 365พอร์ทัลหลัก หรือไม่สามารถเปลี่ยนชื่อผู้ใช้หรือที่อยู่อีเมลได้ เมื่อต้องการแก้ไขปัญหานี้ ให้ตั้งค่า UserPrincipalName ด้วยตนเองโดยใช้สั่ง PowerShell นี้

**ตัวอย่าง: เปลี่ยนชื่อผู้ใช้**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Command นี้จะเปลี่ยนชื่อ davidc@contoso.com เป็น davidchew@contoso.com

For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).