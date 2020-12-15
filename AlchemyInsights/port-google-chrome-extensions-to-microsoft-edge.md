---
title: ส่วนขยายของพอร์ต Google Chrome ไปยัง Microsoft Edge (โครเมียม)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678979"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="2811d-102">ส่วนขยายของพอร์ต Google Chrome ไปยัง Microsoft Edge (โครเมียม)</span><span class="sxs-lookup"><span data-stu-id="2811d-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="2811d-103">ง่ายต่อการ[พอร์ต Google Chrome ส่วนขยายไปยัง Microsoft Edge (โครเมียม)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)</span><span class="sxs-lookup"><span data-stu-id="2811d-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="2811d-104">ในกรณีส่วนใหญ่จะมีการเปลี่ยนแปลงน้อยที่สุดเท่านั้นที่จำเป็นสำหรับการเรียกใช้นามสกุลเหล่านี้บน Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2811d-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="2811d-105">ส่วนขยาย APIs และคีย์แสดงรายการที่ได้รับการสนับสนุนโดย Google Chrome คือรหัสที่เข้ากันได้กับ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2811d-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="2811d-106">อย่างไรก็ตาม Microsoft Edge ไม่สนับสนุนส่วนขยาย APIs gcm, chrome. getAccounts, chrome. getAuthToken และ chrome สแตนซ์</span><span class="sxs-lookup"><span data-stu-id="2811d-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>