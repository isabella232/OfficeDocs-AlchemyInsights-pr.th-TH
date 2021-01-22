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
# <a name="turn-on-ndi-technology"></a>เปิดใช้งานเทคโนโลยี NDI

เทคโนโลยี NDI ต้องเปิดใช้งานสองขั้นตอนกับผู้ใช้ ดังนี้

1. ผู้ดูแลระบบผู้เช่าต้องเปิดใช้งานคุณสมบัติ 'AllowNDIStreaming' ใน CsTeamsMeetingPolicy

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. หลังจากสร้างการเปลี่ยนแปลงนี้ผู้ใช้ต้องเปิดใช้งาน NDI®เทคโนโลยีไคลเอ็นต์เฉพาะของพวกเขาจาก **การตั้งค่า>สิทธิ์**

ดูข้อมูลเพิ่มเติมในการใช้เทคโนโลยี[NDI ใน Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
