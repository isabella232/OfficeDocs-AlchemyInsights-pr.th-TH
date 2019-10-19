---
title: การรีเฟรชโดยใช้ตัวเชื่อมต่อเว็บทำงานไม่ถูกต้อง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1316"
- "2500002"
ms.openlocfilehash: 6bee3c3d0d07f79823fe8683e0bfef33ae6dfdfc
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748919"
---
# <a name="refresh-using-web-connector-doesnt-work-properly"></a><span data-ttu-id="8f258-102">การรีเฟรชโดยใช้ตัวเชื่อมต่อเว็บทำงานไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="8f258-102">Refresh using Web connector doesn't work properly</span></span>

<span data-ttu-id="8f258-103">ถ้าคุณมีสคริปต์ตัวเชื่อมต่อเว็บที่ใช้ฟังก์ชัน[เว็บเพจ](https://msdn.microsoft.com/library/mt260924.aspx)และคุณได้ปรับปรุงชุดข้อมูลหรือรายงานของคุณหลังจากวันที่18พฤศจิกายน๒๐๑๖คุณจำเป็นต้องใช้เกตเวย์เพื่อให้รีเฟรชทำงานได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="8f258-103">If you have a web connector script that's using the [Web.Page](https://msdn.microsoft.com/library/mt260924.aspx) function, and you have updated your dataset or report after November 18th, 2016, you need to use a gateway in order for refresh to work properly.</span></span>

<span data-ttu-id="8f258-104">สำหรับข้อมูลเพิ่มเติม:[https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios](https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios)</span><span class="sxs-lookup"><span data-stu-id="8f258-104">For more information: [https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios](https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios)</span></span>
