---
title: ความต้องการรหัสผ่านที่คาดเดายากของการเปลี่ยนแปลง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701602"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="f8896-102">ความต้องการรหัสผ่านที่คาดเดายากของการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="f8896-102">Change strong password requirement</span></span>

<span data-ttu-id="f8896-103">ต้องใช้รหัสผ่านที่คาดเดายาก โดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f8896-103">Strong passwords are required by default.</span></span> 

<span data-ttu-id="f8896-104">ใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสำหรับผู้ใช้ที่ระบุด้วยคำสั่งนี้:</span><span class="sxs-lookup"><span data-stu-id="f8896-104">Using PowerShell you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="f8896-105">*ชุด MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="f8896-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="f8896-106">ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="f8896-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="f8896-107">วิธีการเชื่อมต่อ O365 กับ PowerShell</span><span class="sxs-lookup"><span data-stu-id="f8896-107">How to connect to O365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="f8896-108">ข้อมูลเพิ่มเติมเกี่ยวกับคำสั่ง PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="f8896-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)