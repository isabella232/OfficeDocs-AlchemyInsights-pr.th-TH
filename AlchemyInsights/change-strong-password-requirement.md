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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="0a8d1-102">เปลี่ยนแปลงความต้องการรหัสผ่านที่คาดเดายาก</span><span class="sxs-lookup"><span data-stu-id="0a8d1-102">Change strong password requirement</span></span>

<span data-ttu-id="0a8d1-103">Microsoft ต้องใช้รหัสผ่านที่คาดเดายากตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="0a8d1-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="0a8d1-104">เมื่อใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดาได้ยากของผู้ใช้ที่ระบุด้วยสั่งเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="0a8d1-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="0a8d1-105">เมื่อต้องการปิดใช้งานรหัสผ่านที่คาดเดายากของผู้ใช้ทั้งหมด ให้ใช้</span><span class="sxs-lookup"><span data-stu-id="0a8d1-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="0a8d1-106">ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="0a8d1-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="0a8d1-107">วิธีเชื่อมต่อกับ Microsoft 365 ด้วย PowerShell</span><span class="sxs-lookup"><span data-stu-id="0a8d1-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="0a8d1-108">ข้อมูลเพิ่มเติมเกี่ยวกับ PowerShell MsolUser สั่ง</span><span class="sxs-lookup"><span data-stu-id="0a8d1-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
