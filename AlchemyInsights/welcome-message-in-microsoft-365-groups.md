---
title: ข้อความต้อนรับในกลุ่มMicrosoft 365ข้อความ
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
- "1200024"
- "5685"
ms.openlocfilehash: 81127b79d4e5a16686ca46d67bfac73c15891938491a702219cd73757c4e106c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997729"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>ข้อความต้อนรับในกลุ่มMicrosoft 365ข้อความ

ผู้ใช้ใหม่ที่Microsoft 365เข้าร่วมกลุ่มจะได้รับอีเมลต้อนรับ ถ้าคุณสมบัติ "UnifiedGroupWelcomedMessageEnabled" เป็นจริง

ในกรณีที่คุณต้องการปิดใช้งานข้อความต้อนรับ ให้ใช้สั่ง [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) ต่อไปนี้:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
