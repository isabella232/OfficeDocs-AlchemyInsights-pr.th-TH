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
# <a name="welcome-message-in-microsoft-365-groups"></a>ข้อความต้อนรับในกลุ่ม Microsoft ๓๖๕

ผู้ใช้ใหม่ที่เข้าร่วม Microsoft ๓๖๕กลุ่มจะได้รับอีเมลที่ยินดีต้อนรับถ้าคุณสมบัติ "UnifiedGroupWelcomeMessageEnabled" เป็น True

ในกรณีที่คุณต้องการปิดใช้งานข้อความต้อนรับให้ใช้คำสั่งของ [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) ต่อไปนี้:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
