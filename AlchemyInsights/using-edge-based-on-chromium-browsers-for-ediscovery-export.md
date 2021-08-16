---
title: การใช้Microsoft Edgeขึ้นอยู่กับChromiumเบราว์เซอร์ของคุณส่งออกของ Ediscovery
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
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998423"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>การใช้Microsoft Edgeขึ้นอยู่กับChromiumเบราว์เซอร์ของคุณส่งออกของ Ediscovery

เนื่องจากการเปลี่ยนแปลงล่าสุด Microsoft Edgeเบราว์เซอร์ของคุณจะไม่เปิดใช้งานClickOnceอีกต่อไปตามค่าเริ่มต้น เมื่อต้องการใช้เครื่องมือส่งออก Microsoft 365 eDiscovery ต่อ คุณจะต้องใช้ Microsoft Internet Explorer หรือเปิดใช้งานการสนับสนุนClickOnceในMicrosoft Edge 

เมื่อต้องการเปิดใช้งานClickOnceการสนับสนุนใน Microsoft EdgeยึดตามChromium: 
1. ในMicrosoft Edgeของคุณ ให้ไปที่ edge://flags/#edge-click-once
2. For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**. 
3. ที่ด้านล่างของหน้าต่างเบราว์เซอร์ ให้เลือก รี **สตาร์** ต <br>
 การเปลี่ยนแปลงจะมีผลหลังจากการรีสตาร์ตMicrosoft Edgeใหม่ 

For information on this and steps for installing the export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).