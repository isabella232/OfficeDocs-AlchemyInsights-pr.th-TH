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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286297"
---
# <a name="change-strong-password-requirement"></a>เปลี่ยนข้อกําหนดรหัสผ่านที่คาดเดายาก

โดยค่าเริ่มต้น Microsoft ต้องใช้รหัสผ่านที่คาดเดายาก 

การใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสําหรับผู้ใช้ที่ระบุโดยใช้คําสั่งนี้:<br>
*ผู้ใช้ชื่อ<UserPrincipalName>–รหัสผ่านที่ต้องใช้รหัสผ่าน$false*

- [ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [วิธีเชื่อมต่อกับ Office 365 ด้วย PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [ข้อมูลเพิ่มเติมเกี่ยวกับคําสั่ง MsolUser PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [ตั้งค่ารหัสผ่านของผู้ใช้แต่ละรายให้ไม่มีวันหมดอายุ](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
