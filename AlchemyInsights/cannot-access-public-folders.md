---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341422"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="24147-102">Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะได้</span><span class="sxs-lookup"><span data-stu-id="24147-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="24147-103">ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทำงานสำหรับผู้ใช้บางรายให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="24147-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="24147-104">เชื่อมต่อกับ EXO PowerShell และกำหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox บนบัญชีผู้ใช้ที่มีปัญหาให้ตรงกับพารามิเตอร์บนบัญชีผู้ใช้ที่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="24147-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="24147-105">ตัวอย่าง</span><span class="sxs-lookup"><span data-stu-id="24147-105">Example:</span></span>

<span data-ttu-id="24147-106">WorkingUser การรับกล่องจดหมาย | ฟุต DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="24147-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="24147-107">การตั้งค่ากล่องจดหมาย ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="24147-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="24147-108">รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="24147-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="24147-109">ถ้าปัญหายังคงอยู่โปรดทำตาม [ขั้นตอน](https://aka.ms/pfcte) ต่อไปนี้เพื่อแก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="24147-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="24147-110">**เมื่อต้องการควบคุมผู้ใช้ที่สามารถเข้าถึงโฟลเดอร์สาธารณะได้โดยใช้ Outlook ให้ทำ**ดังนี้</span><span class="sxs-lookup"><span data-stu-id="24147-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="24147-111">ใช้การตั้งค่า-Set-casmailbox cmdlethttps <mailboxname> -PublicFolderClientAccess $true หรือ $false</span><span class="sxs-lookup"><span data-stu-id="24147-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="24147-112">$true: อนุญาตให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="24147-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="24147-113">$false: ป้องกันไม่ให้ผู้ใช้เข้าถึงโฟลเดอร์สาธารณะใน Outlook</span><span class="sxs-lookup"><span data-stu-id="24147-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="24147-114">นี่เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="24147-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="24147-115">ตั้งค่า-ชื่อ get-organizationconfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="24147-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="24147-116">**หมายเหตุ:** กระบวนงานนี้สามารถควบคุมการเชื่อมต่อได้เฉพาะกับไคลเอ็นต์ Outlook บนเดสก์ท็อปสำหรับ Windows เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="24147-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="24147-117">ผู้ใช้สามารถเข้าถึงโฟลเดอร์สาธารณะได้อย่างต่อเนื่องโดยใช้ OWA หรือ Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="24147-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="24147-118">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ประกาศการสนับสนุนสำหรับการควบคุมการเชื่อมต่อไปยังโฟลเดอร์สาธารณะใน Outlook](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="24147-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>