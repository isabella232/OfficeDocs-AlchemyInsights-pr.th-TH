---
title: ความต้องการรหัสผ่านที่คาดเดายากของการเปลี่ยนแปลง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518778"
---
# <a name="change-strong-password-requirement"></a>ความต้องการรหัสผ่านที่คาดเดายากของการเปลี่ยนแปลง

Microsoft ต้องการรหัสผ่านที่คาดเดายาก โดยค่าเริ่มต้น 

ใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสำหรับผู้ใช้ที่ระบุด้วยคำสั่งนี้:<br>
*ชุด MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีการเชื่อมต่อกับ Office 365 ด้วย PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับคำสั่ง PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)