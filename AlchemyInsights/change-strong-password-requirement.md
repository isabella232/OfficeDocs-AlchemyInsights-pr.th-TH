---
title: เปลี่ยนความต้องการรหัสผ่านที่คาดเดาได้
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804442"
---
# <a name="change-strong-password-requirement"></a>เปลี่ยนความต้องการรหัสผ่านที่คาดเดาได้

ไมโครซอฟท์จำเป็นต้องใช้รหัสผ่านที่คาดเดาได้ตามค่าเริ่มต้น

การใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสำหรับผู้ใช้ที่เฉพาะเจาะจงที่มีคำสั่งเหล่านี้:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

เมื่อต้องการปิดใช้งานรหัสผ่านที่คาดเดายากสำหรับผู้ใช้ทั้งหมดให้ใช้:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีการเชื่อมต่อกับ Microsoft ๓๖๕กับ PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับคำสั่ง PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
