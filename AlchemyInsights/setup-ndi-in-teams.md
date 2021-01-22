---
title: เปิดใช้งานเทคโนโลยี NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935195"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="e1ac8-102">เปิดใช้งานเทคโนโลยี NDI</span><span class="sxs-lookup"><span data-stu-id="e1ac8-102">Turn on NDI technology</span></span>

<span data-ttu-id="e1ac8-103">เทคโนโลยี NDI ต้องเปิดใช้งานสองขั้นตอนกับผู้ใช้ ดังนี้</span><span class="sxs-lookup"><span data-stu-id="e1ac8-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="e1ac8-104">ผู้ดูแลระบบผู้เช่าต้องเปิดใช้งานคุณสมบัติ 'AllowNDIStreaming' ใน CsTeamsMeetingPolicy</span><span class="sxs-lookup"><span data-stu-id="e1ac8-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="e1ac8-105">หลังจากสร้างการเปลี่ยนแปลงนี้ผู้ใช้ต้องเปิดใช้งาน NDI®เทคโนโลยีไคลเอ็นต์เฉพาะของพวกเขาจาก **การตั้งค่า>สิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="e1ac8-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="e1ac8-106">ดูข้อมูลเพิ่มเติมในการใช้เทคโนโลยี[NDI ใน Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="e1ac8-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
