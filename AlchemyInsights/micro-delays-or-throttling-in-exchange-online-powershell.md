---
title: ความล่าช้าของ Micro หรือการควบคุมปริมาณใน Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743933"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="9cbb3-102">ความล่าช้าของ Micro หรือการควบคุมปริมาณใน Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="9cbb3-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="9cbb3-103">คุณอาจเห็นคำเตือน "การหน่วงเวลา Micro ที่นำไปใช้" หรือความล่าช้าเมื่อคุณเรียกใช้สคริปต์และ cmdlets ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="9cbb3-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="9cbb3-104">ต่อไปนี้คือคำแนะนำที่เกี่ยวข้องกับคำแนะนำดังนี้</span><span class="sxs-lookup"><span data-stu-id="9cbb3-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="9cbb3-105">คุณอาจต้องการลองใช้ [โมดูล PowerShell ของ Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ซึ่งรวมถึง cmdlet ที่ยึดตาม REST API และมีมีประสิทธิภาพเพิ่มเติมอย่างมาก</span><span class="sxs-lookup"><span data-stu-id="9cbb3-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="9cbb3-106">นี่อาจเป็นโซลูชันที่ยอดเยี่ยมสำหรับการใช้ Cmdlet ของการรับที่ใช้บ่อย</span><span class="sxs-lookup"><span data-stu-id="9cbb3-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="9cbb3-107">ถ้าคุณจำเป็นต้องใช้ CMDlets ที่ไม่ได้รับการคุ้มครองในโมดูล v2 โปรดดูที่การ [เรียกใช้ cmdlet ของ powershell สำหรับผู้ใช้จำนวนมากใน Office ๓๖๕](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ซึ่งจะอธิบายเกี่ยวกับวิธีการใช้งานการจำกัดปริมาณการควบคุม powershell ที่คาดไว้ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="9cbb3-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
