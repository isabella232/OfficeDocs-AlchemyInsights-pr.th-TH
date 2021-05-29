---
title: ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702145"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a8e4c-102">ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a8e4c-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a8e4c-103">คุณอาจเห็นคําเตือนหรือความล่าช้าของไมโครหน่วงเวลาเมื่อคุณเรียกใช้สคริปต์และ cmdlets Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a8e4c-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a8e4c-104">ต่อไปนี้เป็นวิธีการแก้ไขปัญหาข้อเสนอแนะบางส่วน:</span><span class="sxs-lookup"><span data-stu-id="a8e4c-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="a8e4c-105">โปรดเรียกใช้การวินิจฉัยของเราเพื่อคลายนโยบายการควบคุมปริมาณ PowerShell ของผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="a8e4c-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="a8e4c-106">วิธีแก้ไขนี้จะแก้ไขปัญหาส่วนใหญ่</span><span class="sxs-lookup"><span data-stu-id="a8e4c-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="a8e4c-107">ถ้ายังไม่สามารถแก้ไขปัญหาได้ ให้ใช้โมดูล[Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ซึ่งมี CMDlet ที่ยึดตาม REST API และมีประสิทธิภาพมากขึ้นอย่างมาก</span><span class="sxs-lookup"><span data-stu-id="a8e4c-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a8e4c-108">ซึ่งอาจเป็นโซลูชันที่ยอดเยี่ยมมากมายของ Get- CMDlet ที่ใช้บ่อย</span><span class="sxs-lookup"><span data-stu-id="a8e4c-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a8e4c-109">ถ้าคุณต้องใช้ CMDlet ที่ไม่ครอบคลุมในโมดูล v2 โปรดดู การเรียกใช้[cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ของ PowerShell ของผู้ใช้หลายคนใน Office 365 ซึ่งจะพูดคุยเกี่ยวกับวิธีใช้งานขีดจํากัดการควบคุมปริมาณของ PowerShell ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a8e4c-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
