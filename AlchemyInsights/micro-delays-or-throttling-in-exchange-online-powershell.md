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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830052"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="222e3-102">ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="222e3-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="222e3-103">คุณอาจเห็นคําเตือนหรือความล่าช้าของ "การหน่วงเวลาขนาดเล็ก" เมื่อคุณเรียกใช้สคริปต์และ cmdlet ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="222e3-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="222e3-104">นี่คือข้อเสนอแนะสองรายการที่เกี่ยวข้องกับสิ่งนี้:</span><span class="sxs-lookup"><span data-stu-id="222e3-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="222e3-105">คุณอาจต้องการลองใช้โมดูล PowerShell ของ [Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ซึ่งรวมถึง CMDlet ที่ใช้ REST API และมีประสิทธิภาพมากกว่าอย่างมาก</span><span class="sxs-lookup"><span data-stu-id="222e3-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="222e3-106">ซึ่งอาจเป็นโซลูชันที่ยอดเยี่ยมมากมายของ Get- CMDlet ที่ใช้บ่อย</span><span class="sxs-lookup"><span data-stu-id="222e3-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="222e3-107">ถ้าคุณต้องใช้ CMDlet ที่ไม่ครอบคลุมในโมดูล v2 โปรดดู การเรียกใช้ [cmdlet ของ PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ของผู้ใช้หลายคนใน Office 365 ซึ่งจะพูดคุยเกี่ยวกับวิธีการรับขีดจํากัดการควบคุมปริมาณของ PowerShell ใน Exchange Online ที่คาดหมาย</span><span class="sxs-lookup"><span data-stu-id="222e3-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
