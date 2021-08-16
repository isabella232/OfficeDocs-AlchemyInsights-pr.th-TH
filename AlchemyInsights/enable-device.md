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
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003511"
---
# <a name="enable-device"></a>เปิดใช้งานอุปกรณ์

**เมื่อต้องการเปิดใช้งานอุปกรณ์โดยใช้สั่ง Powershell**

เรียกใช้คำสั่งต่อไปนี้

- เมื่อต้องการรับวัตถุอุปกรณ์: `Get-MsolDevice -Name <Name>`
- เมื่อต้องการเปิดใช้งานอุปกรณ์: `Enable-MsolDevice -DeviceId <DeviceId>`

For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
