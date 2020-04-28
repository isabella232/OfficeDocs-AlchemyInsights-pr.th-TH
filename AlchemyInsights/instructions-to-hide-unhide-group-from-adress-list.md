---
title: คําแนะนําในการซ่อน/ยกเลิกการซ่อนกลุ่มจากรายการที่อยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908363"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>ซ่อนกลุ่ม Microsoft 365 จากรายการที่อยู่ (GAL)

เมื่อต้องการซ่อนกลุ่ม Microsoft 365 จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (เช่น Outlook หรือ OWA), ใช้คําสั่งต่อไปนี้ในเชลล์ของ EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

เมื่อต้องการซ่อนกลุ่ม Microsoft 365 จากการถูกมองเห็นได้ไปยังไคลเอนต์ Exchange ใช้คําสั่งต่อไปนี้ในเชลล์ของ EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

