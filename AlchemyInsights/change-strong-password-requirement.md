---
title: เปลี่ยนข้อกําหนดรหัสผ่านที่คาดเดายาก
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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706580"
---
# <a name="change-strong-password-requirement"></a>เปลี่ยนข้อกําหนดรหัสผ่านที่คาดเดายาก

โดยค่าเริ่มต้น Microsoft ต้องใช้รหัสผ่านที่คาดเดายาก 

การใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสําหรับผู้ใช้ที่ระบุโดยใช้คําสั่งนี้:<br>
*ผู้ใช้ชื่อ<UserPrincipalName>–รหัสผ่านที่ต้องใช้รหัสผ่าน$false*

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีการเชื่อมต่อไปยัง Microsoft 365 ด้วย PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับคําสั่ง MsolUser PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
