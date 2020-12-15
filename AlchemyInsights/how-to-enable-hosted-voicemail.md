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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679163"
---
# <a name="how-to-enable-hosted-voicemail"></a>วิธีการเปิดใช้งานข้อความเสียงที่โฮสต์

เมื่อต้องการเปิดใช้งานข้อความเสียง **HostedVoicemail** ต้องถูกตั้งค่าเป็น $true

คุณสมบัติ **HostedVoicemail** บนผู้ใช้ที่ใช้ PowerShell ระยะไกล (RPS)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเชื่อมต่อกับ RPS ให้ดูที่ [ภาพรวมของ Microsoft Team PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเชื่อมต่อกับ RPS

1. ผู้ดูแลระบบทีมควรเข้าสู่ระบบ PowerShell ระยะไกลสำหรับทีม
1. จาก PowerShell พร้อมท์ผู้ดูแลระบบทีมสามารถเรียกใช้การ **ตั้งค่า-csuser user@contoso.com-HostedVoiceMail $true** ที่ uri sip คือของผู้ใช้ที่มีคำถาม

> [!NOTE]
> การเปลี่ยนแปลงที่เกิดขึ้นกับนโยบายอาจใช้เวลาถึง24ชั่วโมงในการทำซ้ำ