---
title: การใช้ Microsoft Edge โดยยึดตามเบราว์เซอร์โครเมียมสำหรับการส่งออก Ediscovery
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
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734534"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="32325-102">การใช้ Microsoft Edge โดยยึดตามเบราว์เซอร์โครเมียมสำหรับการส่งออก Ediscovery</span><span class="sxs-lookup"><span data-stu-id="32325-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="32325-103">เนื่องจากการเปลี่ยนแปลงล่าสุดเบราว์เซอร์ Microsoft Edge จะไม่มีการสนับสนุน ClickOnce ที่เปิดใช้งานตามค่าเริ่มต้นอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="32325-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="32325-104">เมื่อต้องการดำเนินการต่อโดยใช้เครื่องมือการส่งออกของ Microsoft ๓๖๕ eDiscovery คุณจะต้องใช้ Microsoft Internet Explorer หรือเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="32325-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="32325-105">เมื่อต้องการเปิดใช้งานการสนับสนุน ClickOnce ใน Microsoft Edge โดยยึดตามโครเมียม:</span><span class="sxs-lookup"><span data-stu-id="32325-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="32325-106">ในเบราว์เซอร์ Microsoft Edge ของคุณให้ไปที่ edge://flags/#edge-คลิก-หนึ่งครั้ง</span><span class="sxs-lookup"><span data-stu-id="32325-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="32325-107">สำหรับตัวเลือกการสนับสนุน ClickOnce ให้เปลี่ยนค่าจาก**ค่าเริ่มต้น**หรือ**ปิด**ใช้งานเพื่อ**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="32325-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="32325-108">ที่ด้านล่างของหน้าต่างเบราว์เซอร์ให้เลือก**เริ่มต้นใหม่**</span><span class="sxs-lookup"><span data-stu-id="32325-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="32325-109">การเปลี่ยนแปลงจะมีผลหลังจากเริ่มการทำงานของ Microsoft Edge ใหม่</span><span class="sxs-lookup"><span data-stu-id="32325-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="32325-110">สำหรับข้อมูลเกี่ยวกับการตั้งค่านี้และขั้นตอนสำหรับการติดตั้งเครื่องมือส่งออกให้ดูที่[ส่งออกผลลัพธ์การค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="32325-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>