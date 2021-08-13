---
title: Microsoft Edgeสตริงตัวแทนผู้ใช้ (เดสก์ท็อป)
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
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976020"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edgeสตริงตัวแทนผู้ใช้ (เดสก์ท็อป)

สตริงตัวแทนผู้ใช้ (UA) สามารถใช้เพื่อตรวจหาเวอร์ชันของเบราว์เซอร์ที่ระบุที่ถูกใช้บนระบบปฏิบัติการบางระบบ เช่นเดียวกับเบราว์เซอร์อื่นๆ Microsoft Edgeจะมีข้อมูลนี้ในส่วนหัว HTTP "ตัวแทนผู้ใช้" เมื่อใดก็ตามที่มีการร้องขอไปยังไซต์ The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".

เราขอแนะให้นักพัฒนาเว็บใช้การตรวจหาฟีเจอร์ทุกครั้งที่เป็นไปได้เพื่อปรับปรุงความสามารถในการรักษาโค้ด ลดความยุ่งยากของโค้ด และลดความเสี่ยงที่รหัสจะแตกหักในกรณีที่สตริง UA อัปเดตในอนาคต

For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).