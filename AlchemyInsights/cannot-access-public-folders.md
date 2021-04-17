---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819531"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="309bc-102">Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="309bc-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="309bc-103">ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ใช้งานได้กับผู้ใช้บางราย ให้ลองวิธีต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="309bc-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="309bc-104">เชื่อมต่อกับ EXO PowerShell และกําหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox บนบัญชีผู้ใช้ที่มีปัญหาให้ตรงกับพารามิเตอร์บนบัญชีผู้ใช้ที่ใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="309bc-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="309bc-105">ตัวอย่าง:</span><span class="sxs-lookup"><span data-stu-id="309bc-105">Example:</span></span>

<span data-ttu-id="309bc-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="309bc-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="309bc-107">Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="309bc-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="309bc-108">รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="309bc-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="309bc-109">ถ้าปัญหายังคงอยู่ โปรดปฏิบัติตาม [กระบวนงานนี้](https://aka.ms/pfcte) เพื่อแก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="309bc-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="309bc-110">**เมื่อต้องการควบคุมว่าผู้ใช้คนใดสามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook:**</span><span class="sxs-lookup"><span data-stu-id="309bc-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="309bc-111">ใช้ Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true หรือ $false</span><span class="sxs-lookup"><span data-stu-id="309bc-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="309bc-112">$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="309bc-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="309bc-113">$false: ป้องกันผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="309bc-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="309bc-114">นี่เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="309bc-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="309bc-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="309bc-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="309bc-116">**หมายเหตุ** กระบวนงานนี้สามารถควบคุมการเชื่อมต่อด้วย Outlook บนเดสก์ท็อปไคลเอ็นต์ Windows เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="309bc-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="309bc-117">ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะต่อไปได้โดยใช้ OWA หรือ Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="309bc-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="309bc-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="309bc-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>