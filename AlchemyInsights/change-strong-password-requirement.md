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
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070703"
---
# <a name="change-strong-password-requirement"></a>เปลี่ยนแปลงความต้องการรหัสผ่านที่คาดเดายาก

Microsoft ต้องใช้รหัสผ่านที่คาดเดายากตามค่าเริ่มต้น

เมื่อใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดาได้ยากของผู้ใช้ที่ระบุด้วยสั่งเหล่านี้:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

เมื่อต้องการปิดใช้งานรหัสผ่านที่คาดเดายากของผู้ใช้ทั้งหมด ให้ใช้

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีการเชื่อมต่อMicrosoft 365ด้วย PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับ PowerShell MsolUser สั่ง](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
