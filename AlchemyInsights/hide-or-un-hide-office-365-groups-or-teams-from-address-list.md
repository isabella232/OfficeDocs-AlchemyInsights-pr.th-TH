---
title: ซ่อนหรือยกเลิกการซ่อนกลุ่ม Office 365 หรือทีมจากรายการที่อยู่
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811475"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>ซ่อนหรือยกเลิกการซ่อนกลุ่ม Office 365 หรือทีมจากรายการที่อยู่

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อนกลุ่ม/ทีม Office 365 จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อนกลุ่ม/ทีม Office365 จากไคลเอ็นต์ Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
