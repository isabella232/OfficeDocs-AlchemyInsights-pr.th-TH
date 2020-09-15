---
title: คำแนะนำในการซ่อน/ยกเลิกการซ่อนกลุ่มจากรายการที่อยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663028"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>ซ่อน Microsoft ๓๖๕กลุ่มจากรายการที่อยู่ (GAL)

เมื่อต้องการซ่อนกลุ่ม Microsoft ๓๖๕จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (เช่น Outlook หรือ OWA) ให้ใช้คำสั่งต่อไปนี้ในเชลล์ของ EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

เมื่อต้องการซ่อนกลุ่ม Microsoft ๓๖๕จากการมองเห็นไคลเอ็นต์ Exchange ให้ใช้คำสั่งต่อไปนี้ในเชลล์ของ EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

