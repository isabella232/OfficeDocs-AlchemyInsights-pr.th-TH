---
title: ไม่สามารถเปลี่ยนชื่อผู้ใช้ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798683"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="a9c94-102">ไม่สามารถเปลี่ยนชื่อผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="a9c94-102">Unable to change UserName</span></span>

<span data-ttu-id="a9c94-103">ในบางกรณีการเปลี่ยนแปลง UPN (UserPrincipalName) ไม่ได้เผยแพร่ไปยัง cloud</span><span class="sxs-lookup"><span data-stu-id="a9c94-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="a9c94-104">คุณอาจได้รับข้อผิดพลาดในการตรวจสอบในพอร์ทัล Office ๓๖๕หรือไม่สามารถเปลี่ยนชื่อผู้ใช้หรือที่อยู่อีเมลได้</span><span class="sxs-lookup"><span data-stu-id="a9c94-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="a9c94-105">เมื่อต้องการแก้ไขปัญหานี้ให้ตั้งค่า UserPrincipalName โดยใช้คำสั่ง PowerShell นี้ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="a9c94-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="a9c94-106">**ตัวอย่าง: เปลี่ยนชื่อผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="a9c94-106">**Example: Rename a user**</span></span>

<span data-ttu-id="a9c94-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a9c94-107">PowerShellCopy</span></span>

<span data-ttu-id="a9c94-108">PS C: \> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="a9c94-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="a9c94-109">คำสั่งนี้จะเปลี่ยนชื่อ davidc@contoso.com เป็น davidchew@contoso.com</span><span class="sxs-lookup"><span data-stu-id="a9c94-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="a9c94-110">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ตั้งค่า MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)</span><span class="sxs-lookup"><span data-stu-id="a9c94-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>