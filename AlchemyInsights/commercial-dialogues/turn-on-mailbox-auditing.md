---
title: เปิดใช้งานการตรวจสอบกล่องจดหมาย
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483546"
---
# <a name="turn-on-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายของผู้ใช้รายเดียวหรือทั้งองค์กร ให้เรียกใช้ cmdlets ต่อไปนี้จาก PowerShell ระยะไกล:

- **ผู้ใช้เดี่ยว**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **องค์กร**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู จัดการการตรวจสอบ](https://go.microsoft.com/fwlink/?linkid=2103668)กล่องจดหมาย