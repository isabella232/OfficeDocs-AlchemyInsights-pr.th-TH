---
title: ไมโครความล่าช้าหรือการควบคุมปริมาณใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948028"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>ไมโครความล่าช้าหรือการควบคุมปริมาณใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน

คุณอาจเห็นคําเตือน "หน่วงเวลาแบบจุลภาคที่นําไปใช้" หรือความล่าช้าเมื่อคุณเรียกใช้สคริปต์และ cmdlet ใน Exchange แบบออนไลน์ ต่อไปนี้เป็นคําแนะนําสองข้อที่เกี่ยวข้องกับเรื่องนี้:

- คุณอาจต้องการลองใช้[โมดูล PowerShell V2 แลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ซึ่งรวมถึง CMDlet ที่ยึดตาม REST API และมี performant มากขึ้นอย่างมาก นี้อาจจะเป็นทางออกที่ดีสําหรับจํานวนมากรับ - CMDlet ที่ใช้บ่อย.
- ถ้าคุณจําเป็นต้องใช้ CMDlets ที่ยังไม่ครอบคลุมในโมดูล v2 ยัง โปรดดู[Cmdlet PowerShell ทํางานสําหรับผู้ใช้จํานวนมากใน Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ซึ่งพูดถึงเกี่ยวกับวิธีการรับขีดจํากัดการควบคุมปริมาณ PowerShell ที่คาดไว้ในการแลกเปลี่ยนแบบออนไลน์
