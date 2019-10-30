---
title: คำแนะนำในการซ่อน/ยกเลิกการซ่อนกลุ่มจากรายการที่อยู่
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768958"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>ซ่อนกลุ่ม Office ๓๖๕จากรายการที่อยู่ (GAL)

เมื่อต้องการซ่อนกลุ่ม Office ๓๖๕จากรายการที่อยู่ (GAL) ของไคลเอนต์ Exchange (เช่น Outlook หรือ OWA) ให้ใช้คำสั่งต่อไปนี้ในการเชลล์ EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

หากต้องการซ่อนกลุ่ม Office ๓๖๕จากการมองเห็นไปยังไคลเอนต์ Exchange ให้ใช้คำสั่งต่อไปนี้ใน EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

