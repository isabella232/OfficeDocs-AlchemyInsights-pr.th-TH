---
title: ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816759"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="73018-102">ควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="73018-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="73018-103">เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="73018-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="73018-104">ใช้ `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="73018-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="73018-105">$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="73018-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="73018-106">$false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="73018-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="73018-107">นี่เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="73018-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="73018-108">หมายเหตุ: กระบวนงานนี้สามารถควบคุมการเชื่อมต่อกับ Outlook บนเดสก์ท็อปของไคลเอ็นต์ Windows เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="73018-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="73018-109">ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะต่อไปได้โดยใช้ OWA หรือ Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="73018-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="73018-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span><span class="sxs-lookup"><span data-stu-id="73018-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
