---
title: ไม่สามารถเปลี่ยนชื่อผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440296"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="fd24b-102">ไม่สามารถเปลี่ยนชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="fd24b-102">Unable to change UserName</span></span>

<span data-ttu-id="fd24b-103">ในบางกรณี การเปลี่ยนแปลง UPN (UserPrincipalName) จะไม่ถูกเผยแพร่ไปยังระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="fd24b-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="fd24b-104">คุณอาจได้รับข้อผิดพลาดในการตรวจสอบความถูกต้องในพอร์ทัล Office 365 หรือไม่สามารถเปลี่ยนชื่อผู้ใช้หรือที่อยู่อีเมลได้</span><span class="sxs-lookup"><span data-stu-id="fd24b-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="fd24b-105">เมื่อต้องการแก้ไขปัญหานี้ ด้วยตนเองตั้งค่า UserPrincipalName โดยใช้คําสั่ง PowerShell นี้</span><span class="sxs-lookup"><span data-stu-id="fd24b-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="fd24b-106">**ตัวอย่าง: เปลี่ยนชื่อผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="fd24b-106">**Example: Rename a user**</span></span>

<span data-ttu-id="fd24b-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="fd24b-107">PowerShellCopy</span></span>

<span data-ttu-id="fd24b-108">PS C: \> ชุด-MsolUserPrincipalName -userprincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="fd24b-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="fd24b-109">คําสั่งนี้เปลี่ยนชื่อdavidc@contoso.comdavidchew@contoso.com</span><span class="sxs-lookup"><span data-stu-id="fd24b-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="fd24b-110">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ชุด MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)</span><span class="sxs-lookup"><span data-stu-id="fd24b-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>