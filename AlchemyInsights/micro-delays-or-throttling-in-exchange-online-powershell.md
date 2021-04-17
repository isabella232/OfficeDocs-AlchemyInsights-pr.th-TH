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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>ความล่าช้าหรือการควบคุมปริมาณใน Exchange Online PowerShell

คุณอาจเห็นคําเตือนหรือความล่าช้าของ "การหน่วงเวลาขนาดเล็ก" เมื่อคุณเรียกใช้สคริปต์และ cmdlet ใน Exchange Online นี่คือข้อเสนอแนะสองรายการที่เกี่ยวข้องกับสิ่งนี้:

- คุณอาจต้องการลองใช้โมดูล PowerShell ของ [Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ซึ่งรวมถึง CMDlet ที่ใช้ REST API และมีประสิทธิภาพมากกว่าอย่างมาก ซึ่งอาจเป็นโซลูชันที่ยอดเยี่ยมมากมายของ Get- CMDlet ที่ใช้บ่อย
- ถ้าคุณต้องใช้ CMDlet ที่ไม่ครอบคลุมในโมดูล v2 โปรดดู การเรียกใช้ [cmdlet ของ PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ของผู้ใช้หลายคนใน Office 365 ซึ่งจะพูดคุยเกี่ยวกับวิธีการรับขีดจํากัดการควบคุมปริมาณของ PowerShell ใน Exchange Online ที่คาดหมาย
