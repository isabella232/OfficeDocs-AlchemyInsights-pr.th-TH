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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314719"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell

คุณอาจเห็นคําเตือนหรือความล่าช้าของไมโครหน่วงเวลาเมื่อคุณเรียกใช้สคริปต์และ cmdlets Exchange Online ต่อไปนี้เป็นวิธีการแก้ไขปัญหาข้อเสนอแนะบางส่วน:

- โปรดเรียกใช้การวินิจฉัยของเราเพื่อคลายนโยบายการควบคุมปริมาณ PowerShell ของผู้เช่าของคุณ วิธีแก้ไขนี้จะแก้ไขปัญหาส่วนใหญ่
- ถ้ายังไม่สามารถแก้ไขปัญหาได้ ให้ใช้โมดูล[Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ซึ่งมี CMDlet ที่ยึดตาม REST API และมีประสิทธิภาพมากขึ้นอย่างมาก ซึ่งอาจเป็นโซลูชันที่ยอดเยี่ยมมากมายของ Get- CMDlet ที่ใช้บ่อย
- ถ้าคุณต้องใช้ CMDlet ที่ไม่ครอบคลุมในโมดูล v2 โปรดดู การเรียกใช้[cmdlet ของ PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ให้กับผู้ใช้หลายคนใน Office 365 ซึ่งจะพูดคุยเกี่ยวกับวิธีใช้งานขีดจํากัดการควบคุมปริมาณของ PowerShell ใน Exchange Online
