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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="799ed-102">ซ่อนหรือยกเลิกการซ่อนกลุ่มหรือกลุ่ม Office 365 จากรายการที่อยู่</span><span class="sxs-lookup"><span data-stu-id="799ed-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="799ed-103">ใช้คําสั่ง POWERShell EXO ต่อไปนี้เพื่อซ่อน หรือยกเลิกการซ่อนกลุ่ม/ทีม Office 365 จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="799ed-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="799ed-104">ใช้คําสั่ง PowerShell EXO ต่อไปนี้เพื่อซ่อน หรือยกเลิกการซ่อนกลุ่ม/ทีม Office365 จากไคลเอ็นต์ของ Exchange (Outlook OWA):</span><span class="sxs-lookup"><span data-stu-id="799ed-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="799ed-105">สําหรับคําแนะนําโดยละเอียด ให้ดูที่[ซ่อนกลุ่ม Office 365 จาก GAL และไคลเอ็นต์ของ Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)</span><span class="sxs-lookup"><span data-stu-id="799ed-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
