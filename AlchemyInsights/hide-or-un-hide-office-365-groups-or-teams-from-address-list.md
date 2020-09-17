---
title: ซ่อนหรือยกเลิกการซ่อนกลุ่ม Office ๓๖๕หรือทีมจากรายการที่อยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782346"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="2e15c-102">ซ่อนหรือยกเลิกการซ่อนกลุ่ม Office ๓๖๕หรือทีมจากรายการที่อยู่</span><span class="sxs-lookup"><span data-stu-id="2e15c-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="2e15c-103">ใช้คำสั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อน Office ๓๖๕กลุ่ม/ทีมจากรายชื่อที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="2e15c-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="2e15c-104">ใช้คำสั่ง EXO PowerShell ต่อไปนี้เพื่อซ่อนหรือยกเลิกการซ่อนกลุ่ม Office365/ทีมจากไคลเอ็นต์ Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="2e15c-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="2e15c-105">สำหรับคำแนะนำโดยละเอียดให้ดู[ที่ซ่อนกลุ่ม Office ๓๖๕จากไคลเอ็นต์ GAL และ Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)</span><span class="sxs-lookup"><span data-stu-id="2e15c-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
