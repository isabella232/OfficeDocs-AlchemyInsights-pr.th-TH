---
title: ข้อความต้อนรับในกลุ่ม Microsoft ๓๖๕
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725858"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="a9d0c-102">ข้อความต้อนรับในกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="a9d0c-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="a9d0c-103">ผู้ใช้ใหม่ที่เข้าร่วม Microsoft ๓๖๕กลุ่มจะได้รับอีเมลที่ยินดีต้อนรับถ้าคุณสมบัติ "UnifiedGroupWelcomeMessageEnabled" เป็น True</span><span class="sxs-lookup"><span data-stu-id="a9d0c-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="a9d0c-104">ในกรณีที่คุณต้องการปิดใช้งานข้อความต้อนรับให้ใช้คำสั่งของ [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a9d0c-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
