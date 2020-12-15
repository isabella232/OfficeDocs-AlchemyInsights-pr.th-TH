---
title: สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)
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
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679331"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="e9c48-102">สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)</span><span class="sxs-lookup"><span data-stu-id="e9c48-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="e9c48-103">สตริงของบริษัทตัวแทนผู้ใช้ (UA) สามารถใช้เพื่อตรวจสอบเวอร์ชันของเบราว์เซอร์ที่เฉพาะเจาะจงกำลังถูกใช้ในระบบปฏิบัติการบางอย่างได้</span><span class="sxs-lookup"><span data-stu-id="e9c48-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="e9c48-104">เช่นเดียวกับเบราว์เซอร์อื่นๆ Microsoft Edge จะรวมข้อมูลนี้ไว้ในส่วนหัว "ตัวแทนผู้ใช้" เมื่อใดก็ตามที่จะทำการร้องขอไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="e9c48-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="e9c48-105">นอกจากนี้คุณยังสามารถเข้าถึงข้อมูลเวอร์ชันของเบราว์เซอร์ผ่านทาง JavaScript ได้โดยการสอบถามค่า "userAgent"</span><span class="sxs-lookup"><span data-stu-id="e9c48-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="e9c48-106">เราขอแนะนำให้นักพัฒนาเว็บทำการใช้การตรวจสอบฟีเจอร์เมื่อใดก็ตามที่เป็นไปได้ในการปรับปรุงรหัสบำรุงลดรหัสเปราะและลดความเสี่ยงของรหัสความแตกแยกในเหตุการณ์ของการอัปเดสตริงที่ UA ในอนาคต</span><span class="sxs-lookup"><span data-stu-id="e9c48-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="e9c48-107">สำหรับข้อมูลเพิ่มเติมให้ดู[สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)</span><span class="sxs-lookup"><span data-stu-id="e9c48-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>