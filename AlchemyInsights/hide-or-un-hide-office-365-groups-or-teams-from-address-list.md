---
title: ซ่อนหรือยกเลิกการซ่อนOffice 365หรือทีมจากรายการที่อยู่
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088415"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>ซ่อนหรือยกเลิกการซ่อนOffice 365หรือทีมจากรายการที่อยู่

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อนกลุ่ม/Office 365จากรายการที่อยู่ (GAL) Exchangeไคลเอ็นต์ (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อนกลุ่ม/ทีม Office365 จากไคลเอ็นต์ Exchangeไคลเอ็นต์ (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
