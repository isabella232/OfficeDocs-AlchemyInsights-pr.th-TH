---
title: คําแนะนําในการซ่อน/ยกเลิกการซ่อนกลุ่มจากรายการที่อยู่
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926264"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>ซ่อนMicrosoft 365ที่ติดต่อจากรายการที่อยู่ (GAL)

เมื่อต้องการซ่อนกลุ่มMicrosoft 365ที่อยู่จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (เช่น Outlook หรือ OWA) ให้ใช้สั่งต่อไปนี้ในเชลล์ EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

เมื่อต้องการซ่อนMicrosoft 365ไคลเอ็นต์ของ Exchangeให้มองเห็น ให้ใช้สั่งต่อไปนี้ใน SHELL EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

