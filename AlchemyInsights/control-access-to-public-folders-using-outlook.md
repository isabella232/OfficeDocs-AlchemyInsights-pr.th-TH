---
title: การควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804004"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="6683c-102">การควบคุมการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="6683c-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="6683c-103">เมื่อต้องการควบคุมผู้ใช้ที่สามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="6683c-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="6683c-104">ใช้ `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="6683c-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="6683c-105">$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="6683c-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="6683c-106">$false: ป้องกันไม่ให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="6683c-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6683c-107">นี่เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="6683c-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="6683c-108">หมายเหตุ: กระบวนการนี้สามารถควบคุมการเชื่อมต่อกับไคลเอ็นต์ Outlook บนเดสก์ท็อปสำหรับ Windows ได้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="6683c-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6683c-109">ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะได้ต่อไปโดยใช้ OWA หรือ Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="6683c-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="6683c-110">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่การควบคุมการเชื่อมต่อไปยังโฟลเดอร์สาธารณะใน Outlook](https://aka.ms/controlpf) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6683c-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
