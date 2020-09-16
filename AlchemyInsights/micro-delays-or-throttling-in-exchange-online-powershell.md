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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>ความล่าช้าของ Micro หรือการควบคุมปริมาณใน Exchange Online PowerShell

คุณอาจเห็นคำเตือน "การหน่วงเวลา Micro ที่นำไปใช้" หรือความล่าช้าเมื่อคุณเรียกใช้สคริปต์และ cmdlets ใน Exchange Online ต่อไปนี้คือคำแนะนำที่เกี่ยวข้องกับคำแนะนำดังนี้

- คุณอาจต้องการลองใช้ [โมดูล PowerShell ของ Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)ซึ่งรวมถึง cmdlet ที่ยึดตาม REST API และมีมีประสิทธิภาพเพิ่มเติมอย่างมาก นี่อาจเป็นโซลูชันที่ยอดเยี่ยมสำหรับการใช้ Cmdlet ของการรับที่ใช้บ่อย
- ถ้าคุณจำเป็นต้องใช้ CMDlets ที่ไม่ได้รับการคุ้มครองในโมดูล v2 โปรดดูที่การ [เรียกใช้ cmdlet ของ powershell สำหรับผู้ใช้จำนวนมากใน Office ๓๖๕](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)ซึ่งจะอธิบายเกี่ยวกับวิธีการใช้งานการจำกัดปริมาณการควบคุม powershell ที่คาดไว้ใน Exchange Online
