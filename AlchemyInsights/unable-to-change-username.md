---
title: ไม่สามารถเปลี่ยนชื่อผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440296"
---
# <a name="unable-to-change-username"></a>ไม่สามารถเปลี่ยนชื่อผู้ใช้

ในบางกรณี การเปลี่ยนแปลง UPN (UserPrincipalName) จะไม่ถูกเผยแพร่ไปยังระบบคลาวด์ คุณอาจได้รับข้อผิดพลาดในการตรวจสอบความถูกต้องในพอร์ทัล Office 365 หรือไม่สามารถเปลี่ยนชื่อผู้ใช้หรือที่อยู่อีเมลได้ เมื่อต้องการแก้ไขปัญหานี้ ด้วยตนเองตั้งค่า UserPrincipalName โดยใช้คําสั่ง PowerShell นี้

**ตัวอย่าง: เปลี่ยนชื่อผู้ใช้**

PowerShellCopy

PS C: \> ชุด-MsolUserPrincipalName -userprincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

คําสั่งนี้เปลี่ยนชื่อdavidc@contoso.comdavidchew@contoso.com

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ชุด MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)