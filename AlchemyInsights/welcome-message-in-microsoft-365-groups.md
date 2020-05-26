---
title: ข้อความต้อนรับในกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358335"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="5e9d3-102">ข้อความต้อนรับในกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5e9d3-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="5e9d3-103">ผู้ใช้ใหม่เข้าร่วมกลุ่ม Microsoft 365 จะได้รับอีเมลต้อนรับถ้าคุณสมบัติ "UnifiedGroupWelcomeMessageEnabled" เป็นจริง</span><span class="sxs-lookup"><span data-stu-id="5e9d3-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="5e9d3-104">ในกรณีที่คุณต้องการปิดการใช้งานข้อความต้อนรับ ให้ใช้คําสั่ง[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5e9d3-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
