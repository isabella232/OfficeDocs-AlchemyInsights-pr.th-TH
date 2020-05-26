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
# <a name="welcome-message-in-microsoft-365-groups"></a>ข้อความต้อนรับในกลุ่ม Microsoft 365

ผู้ใช้ใหม่เข้าร่วมกลุ่ม Microsoft 365 จะได้รับอีเมลต้อนรับถ้าคุณสมบัติ "UnifiedGroupWelcomeMessageEnabled" เป็นจริง

ในกรณีที่คุณต้องการปิดการใช้งานข้อความต้อนรับ ให้ใช้คําสั่ง[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ต่อไปนี้:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
