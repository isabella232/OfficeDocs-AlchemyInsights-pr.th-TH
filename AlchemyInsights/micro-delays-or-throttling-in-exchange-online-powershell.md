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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell

คุณอาจเห็นคําเตือนหรือความล่าช้าของไมโครหน่วงเวลาเมื่อคุณเรียกใช้สคริปต์และ cmdlets Exchange Online ต่อไปนี้เป็นวิธีการแก้ไขปัญหาข้อเสนอแนะบางส่วน:

- โปรดเรียกใช้การวินิจฉัยของเราเพื่อคลายนโยบายการควบคุมปริมาณ PowerShell ของผู้เช่าของคุณ วิธีแก้ไขนี้จะแก้ไขปัญหาส่วนใหญ่
- ถ้ายังไม่สามารถแก้ไขปัญหาได้ ให้ใช้โมดูล[Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ซึ่งมี CMDlet ที่ยึดตาม REST API และมีประสิทธิภาพมากขึ้นอย่างมาก ซึ่งอาจเป็นโซลูชันที่ยอดเยี่ยมมากมายของ Get- CMDlet ที่ใช้บ่อย
- ถ้าคุณต้องใช้ CMDlet ที่ไม่ครอบคลุมในโมดูล v2 โปรดดู การเรียกใช้[cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ของ PowerShell ของผู้ใช้หลายคนใน Office 365 ซึ่งจะพูดคุยเกี่ยวกับวิธีใช้งานขีดจํากัดการควบคุมปริมาณของ PowerShell ใน Exchange Online
