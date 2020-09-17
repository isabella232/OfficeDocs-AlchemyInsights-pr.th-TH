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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798683"
---
# <a name="unable-to-change-username"></a>ไม่สามารถเปลี่ยนชื่อผู้ใช้ได้

ในบางกรณีการเปลี่ยนแปลง UPN (UserPrincipalName) ไม่ได้เผยแพร่ไปยัง cloud คุณอาจได้รับข้อผิดพลาดในการตรวจสอบในพอร์ทัล Office ๓๖๕หรือไม่สามารถเปลี่ยนชื่อผู้ใช้หรือที่อยู่อีเมลได้ เมื่อต้องการแก้ไขปัญหานี้ให้ตั้งค่า UserPrincipalName โดยใช้คำสั่ง PowerShell นี้ด้วยตนเอง

**ตัวอย่าง: เปลี่ยนชื่อผู้ใช้**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

คำสั่งนี้จะเปลี่ยนชื่อ davidc@contoso.com เป็น davidchew@contoso.com

สำหรับข้อมูลเพิ่มเติมให้ดูที่[ตั้งค่า MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)