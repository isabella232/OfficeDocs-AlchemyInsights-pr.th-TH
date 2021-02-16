---
title: เปิดใช้งานอุปกรณ์
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256987"
---
# <a name="enable-device"></a>เปิดใช้งานอุปกรณ์

**เมื่อต้องการเปิดใช้งานอุปกรณ์โดยใช้สั่ง Powershell**

เรียกใช้คำสั่งต่อไปนี้

- เมื่อต้องการรับวัตถุอุปกรณ์: `Get-MsolDevice -Name <Name>`
- เมื่อต้องการเปิดใช้งานอุปกรณ์: `Enable-MsolDevice -DeviceId <DeviceId>`

For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
