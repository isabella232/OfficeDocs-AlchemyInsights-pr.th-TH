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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="e1a9d-102">เปลี่ยนข้อกําหนดรหัสผ่านที่คาดเดายาก</span><span class="sxs-lookup"><span data-stu-id="e1a9d-102">Change strong password requirement</span></span>

<span data-ttu-id="e1a9d-103">โดยค่าเริ่มต้น Microsoft ต้องใช้รหัสผ่านที่คาดเดายาก</span><span class="sxs-lookup"><span data-stu-id="e1a9d-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="e1a9d-104">การใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสําหรับผู้ใช้ที่ระบุโดยใช้คําสั่งนี้:</span><span class="sxs-lookup"><span data-stu-id="e1a9d-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="e1a9d-105">*ผู้ใช้ชื่อ<UserPrincipalName>–รหัสผ่านที่ต้องใช้รหัสผ่าน$false*</span><span class="sxs-lookup"><span data-stu-id="e1a9d-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="e1a9d-106">ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="e1a9d-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="e1a9d-107">วิธีเชื่อมต่อกับ Office 365 ด้วย PowerShell</span><span class="sxs-lookup"><span data-stu-id="e1a9d-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="e1a9d-108">ข้อมูลเพิ่มเติมเกี่ยวกับคําสั่ง MsolUser PowerShell</span><span class="sxs-lookup"><span data-stu-id="e1a9d-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="e1a9d-109">ตั้งค่ารหัสผ่านของผู้ใช้แต่ละรายให้ไม่มีวันหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="e1a9d-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
