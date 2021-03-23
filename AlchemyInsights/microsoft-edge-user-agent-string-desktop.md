---
title: สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8221"
- "9004596"
ms.openlocfilehash: 42c39f5661f57c7b57fa471f9c204e5c27f2f214
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037300"
---
# <a name="microsoft-edge-user-agent-strings-desktop"></a><span data-ttu-id="2ce1d-102">สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)</span><span class="sxs-lookup"><span data-stu-id="2ce1d-102">Microsoft Edge user agent strings (Desktop)</span></span>

<span data-ttu-id="2ce1d-103">สตริงตัวแทนผู้ใช้ (UA) สามารถใช้เพื่อตรวจสอบเวอร์ชันของเบราว์เซอร์ที่ระบุที่ถูกใช้บนระบบปฏิบัติการบางระบบ</span><span class="sxs-lookup"><span data-stu-id="2ce1d-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="2ce1d-104">เช่นเดียวกับเบราว์เซอร์อื่นๆ Microsoft Edge จะรวมข้อมูลนี้ในส่วนหัว HTTP "ตัวแทนผู้ใช้" เมื่อใดก็ตามที่มีการร้องขอไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="2ce1d-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="2ce1d-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span><span class="sxs-lookup"><span data-stu-id="2ce1d-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="2ce1d-106">เราขอแนะให้นักพัฒนาเว็บใช้การตรวจหาฟีเจอร์เมื่อใดก็ตามที่เป็นไปได้เพื่อปรับปรุงความสามารถในการรักษาโค้ด ลดความหงุดหงิดของโค้ด และลดความเสี่ยงของรหัสที่แตกหักในกรณีที่การอัปเดตสตริง UA ในอนาคต</span><span class="sxs-lookup"><span data-stu-id="2ce1d-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="2ce1d-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="2ce1d-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>

