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
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>การใช้ Microsoft Edge ที่ใช้เบราว์เซอร์ Chromium เพื่อส่งออก Ediscovery

เนื่องจากการเปลี่ยนแปลงล่าสุด เบราว์เซอร์ Microsoft Edge จะไม่เปิดใช้งานการสนับสนุน ClickOnce ตามค่าเริ่มต้นอีกต่อไป เมื่อต้องการใช้เครื่องมือส่งออก eDiscovery ของ Microsoft 365 ต่อ คุณจะต้องใช้ Microsoft Internet Explorer หรือเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge 

เมื่อต้องการเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge ที่ยึดตาม Chromium: 
1. ในเบราว์เซอร์ Microsoft Edge ให้ไปที่ edge://flags/#edge-click-once
2. For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**. 
3. ที่ด้านล่างของหน้าต่างเบราว์เซอร์ ให้เลือก รี **สตาร์** ต <br>
 การเปลี่ยนแปลงจะมีผลหลังจากรีสตาร์ต Microsoft Edge 

For information on this and steps for installing the export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).