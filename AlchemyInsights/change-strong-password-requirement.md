---
title: เปลี่ยนแปลงการกําหนดรหัสผ่านที่คาดเดายาก
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818487"
---
# <a name="change-strong-password-requirement"></a>เปลี่ยนแปลงความต้องการรหัสผ่านที่คาดเดายาก

Microsoft ต้องใช้รหัสผ่านที่คาดเดายากตามค่าเริ่มต้น

เมื่อใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดาได้ยากของผู้ใช้ที่ระบุด้วยสั่งเหล่านี้:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

เมื่อต้องการปิดใช้งานรหัสผ่านที่คาดเดายากของผู้ใช้ทั้งหมด ให้ใช้

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีเชื่อมต่อกับ Microsoft 365 ด้วย PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับ PowerShell MsolUser สั่ง](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
