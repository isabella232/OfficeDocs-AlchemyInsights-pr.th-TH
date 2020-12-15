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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="17890-102">วิธีการเปิดใช้งานข้อความเสียงที่โฮสต์</span><span class="sxs-lookup"><span data-stu-id="17890-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="17890-103">เมื่อต้องการเปิดใช้งานข้อความเสียง **HostedVoicemail** ต้องถูกตั้งค่าเป็น $true</span><span class="sxs-lookup"><span data-stu-id="17890-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="17890-104">คุณสมบัติ **HostedVoicemail** บนผู้ใช้ที่ใช้ PowerShell ระยะไกล (RPS)</span><span class="sxs-lookup"><span data-stu-id="17890-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="17890-105">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเชื่อมต่อกับ RPS ให้ดูที่ [ภาพรวมของ Microsoft Team PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเชื่อมต่อกับ RPS</span><span class="sxs-lookup"><span data-stu-id="17890-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="17890-106">ผู้ดูแลระบบทีมควรเข้าสู่ระบบ PowerShell ระยะไกลสำหรับทีม</span><span class="sxs-lookup"><span data-stu-id="17890-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="17890-107">จาก PowerShell พร้อมท์ผู้ดูแลระบบทีมสามารถเรียกใช้การ **ตั้งค่า-csuser user@contoso.com-HostedVoiceMail $true** ที่ uri sip คือของผู้ใช้ที่มีคำถาม</span><span class="sxs-lookup"><span data-stu-id="17890-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="17890-108">การเปลี่ยนแปลงที่เกิดขึ้นกับนโยบายอาจใช้เวลาถึง24ชั่วโมงในการทำซ้ำ</span><span class="sxs-lookup"><span data-stu-id="17890-108">Changes to policies can take up to 24 hours to replicate.</span></span>