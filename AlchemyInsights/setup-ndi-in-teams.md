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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023541"
---
# <a name="turn-on-ndi-technology"></a>เปิดใช้งานเทคโนโลยี NDI

เทคโนโลยี NDI ต้องมีสองขั้นตอนในการเปิดให้กับผู้ใช้ ดังนี้

1. ผู้ดูแลระบบผู้เช่าต้องเปิดใช้งานคุณสมบัติ 'AllowNDIStreaming' ใน CsTeamsMeetingPolicy

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. หลังจากสร้างการเปลี่ยนแปลงนี้ผู้ใช้ต้องเปิดใช้งาน NDI®ของไคลเอ็นต์เฉพาะจากการตั้งค่า >**สิทธิ์** ของพวกเขา

For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
