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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681891"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="3b657-102">เปลี่ยนความต้องการรหัสผ่านที่คาดเดาได้</span><span class="sxs-lookup"><span data-stu-id="3b657-102">Change strong password requirement</span></span>

<span data-ttu-id="3b657-103">ไมโครซอฟท์จำเป็นต้องใช้รหัสผ่านที่คาดเดาได้ตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="3b657-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="3b657-104">การใช้ PowerShell คุณสามารถปิดใช้งานรหัสผ่านที่คาดเดายากสำหรับผู้ใช้ที่เฉพาะเจาะจงด้วยคำสั่งนี้:</span><span class="sxs-lookup"><span data-stu-id="3b657-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="3b657-105">*ตั้งค่า-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="3b657-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="3b657-106">ข้อมูลเพิ่มเติมเกี่ยวกับนโยบายรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="3b657-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="3b657-107">วิธีการเชื่อมต่อกับ Microsoft ๓๖๕กับ PowerShell</span><span class="sxs-lookup"><span data-stu-id="3b657-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="3b657-108">ข้อมูลเพิ่มเติมเกี่ยวกับคำสั่ง PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="3b657-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
