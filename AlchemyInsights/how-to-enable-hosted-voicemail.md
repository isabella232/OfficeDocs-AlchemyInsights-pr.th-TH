---
title: วิธีการเปิดใช้งานข้อความเสียงที่โฮสต์
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318667"
---
# <a name="how-to-enable-hosted-voicemail"></a>วิธีการเปิดใช้งานข้อความเสียงที่โฮสต์

เมื่อต้องการเปิดใช้งานข้อความเสียง **HostedVoicemail** ต้องตั้งค่า$trueข้อความ

คุณสมบัติ **HostedVoicemail** บนผู้ใช้ที่ใช้ Remote PowerShell (RPS)

For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.

1. ผู้ดูแลระบบ Teams ควรเข้าสู่ระบบ PowerShell ระยะไกล Teams
1. จากพร้อมท์ PowerShell Teams ผู้ดูแลระบบสามารถเรียกใช้ **set-csuser user@contoso.com -HostedVoiceMail $true** โดยที่ sip uri เป็นของผู้ใช้ในคําถาม

**หมายเหตุ**: การเปลี่ยนแปลงนโยบายอาจใช้เวลาถึง 24 ชั่วโมงในการสลองได้