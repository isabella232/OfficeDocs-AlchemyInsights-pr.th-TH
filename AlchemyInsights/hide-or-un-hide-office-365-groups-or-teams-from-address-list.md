---
title: ซ่อนหรือยกเลิกการซ่อนกลุ่มหรือกลุ่ม Office 365 จากรายการที่อยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225570"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>ซ่อนหรือยกเลิกการซ่อนกลุ่มหรือกลุ่ม Office 365 จากรายการที่อยู่

ใช้คําสั่ง POWERShell EXO ต่อไปนี้เพื่อซ่อน หรือยกเลิกการซ่อนกลุ่ม/ทีม Office 365 จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

ใช้คําสั่ง PowerShell EXO ต่อไปนี้เพื่อซ่อน หรือยกเลิกการซ่อนกลุ่ม/ทีม Office365 จากไคลเอ็นต์ของ Exchange (Outlook OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- สําหรับคําแนะนําโดยละเอียด ให้ดูที่[ซ่อนกลุ่ม Office 365 จาก GAL และไคลเอ็นต์ของ Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
