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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055573"
---
# <a name="how-to-enable-hosted-voicemail"></a>วิธีการเปิดใช้งานข้อความเสียงที่โฮสต์

เมื่อต้องการเปิดใช้งานข้อความเสียง **HostedVoicemail** ต้องตั้งค่า$trueข้อความ

คุณสมบัติ **HostedVoicemail** บนผู้ใช้ที่ใช้ Remote PowerShell (RPS)

For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.

1. ผู้ดูแลระบบTeamsควรเข้าสู่ระบบ PowerShell ระยะไกล Teamsของคุณ
1. From PowerShell prompt the Teams admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.

> [!NOTE]
> การเปลี่ยนแปลงนโยบายอาจใช้เวลาถึง 24 ชั่วโมงในการสลองได้