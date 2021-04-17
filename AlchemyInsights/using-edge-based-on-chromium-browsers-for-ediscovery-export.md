---
title: การใช้ Microsoft Edge ที่ใช้เบราว์เซอร์ Chromium เพื่อส่งออก Ediscovery
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834390"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="af701-102">การใช้ Microsoft Edge ที่ใช้เบราว์เซอร์ Chromium เพื่อส่งออก Ediscovery</span><span class="sxs-lookup"><span data-stu-id="af701-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="af701-103">เนื่องจากการเปลี่ยนแปลงล่าสุด เบราว์เซอร์ Microsoft Edge จะไม่เปิดใช้งานการสนับสนุน ClickOnce ตามค่าเริ่มต้นอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="af701-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="af701-104">เมื่อต้องการใช้เครื่องมือส่งออก eDiscovery ของ Microsoft 365 ต่อ คุณจะต้องใช้ Microsoft Internet Explorer หรือเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="af701-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="af701-105">เมื่อต้องการเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge ที่ยึดตาม Chromium:</span><span class="sxs-lookup"><span data-stu-id="af701-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="af701-106">ในเบราว์เซอร์ Microsoft Edge ให้ไปที่ edge://flags/#edge-click-once</span><span class="sxs-lookup"><span data-stu-id="af701-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="af701-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span><span class="sxs-lookup"><span data-stu-id="af701-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="af701-108">ที่ด้านล่างของหน้าต่างเบราว์เซอร์ ให้เลือก รี **สตาร์** ต</span><span class="sxs-lookup"><span data-stu-id="af701-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="af701-109">การเปลี่ยนแปลงจะมีผลหลังจากรีสตาร์ต Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="af701-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="af701-110">For information on this and steps for installing the export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="af701-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>