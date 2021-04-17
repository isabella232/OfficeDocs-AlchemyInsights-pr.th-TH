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
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831897"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="c6a59-102">ซ่อนกลุ่ม Microsoft 365 จากรายการที่อยู่ (GAL)</span><span class="sxs-lookup"><span data-stu-id="c6a59-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="c6a59-103">เมื่อต้องการซ่อนกลุ่ม Microsoft 365 จากรายการที่อยู่ (GAL) ของไคลเอ็นต์ Exchange (เช่น Outlook หรือ OWA) ให้ใช้สั่งต่อไปนี้ใน SHELL EXO:</span><span class="sxs-lookup"><span data-stu-id="c6a59-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="c6a59-104">เมื่อต้องการซ่อนกลุ่ม Microsoft 365 จากที่สามารถมองเห็นได้ในไคลเอ็นต์ Exchange ให้ใช้สั่งต่อไปนี้ในเชลล์ EXO:</span><span class="sxs-lookup"><span data-stu-id="c6a59-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

