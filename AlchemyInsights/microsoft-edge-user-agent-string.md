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
# <a name="microsoft-edge-user-agent-string-desktop"></a>สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)

สตริงของบริษัทตัวแทนผู้ใช้ (UA) สามารถใช้เพื่อตรวจสอบเวอร์ชันของเบราว์เซอร์ที่เฉพาะเจาะจงกำลังถูกใช้ในระบบปฏิบัติการบางอย่างได้ เช่นเดียวกับเบราว์เซอร์อื่นๆ Microsoft Edge จะรวมข้อมูลนี้ไว้ในส่วนหัว "ตัวแทนผู้ใช้" เมื่อใดก็ตามที่จะทำการร้องขอไปยังไซต์ นอกจากนี้คุณยังสามารถเข้าถึงข้อมูลเวอร์ชันของเบราว์เซอร์ผ่านทาง JavaScript ได้โดยการสอบถามค่า "userAgent"

เราขอแนะนำให้นักพัฒนาเว็บทำการใช้การตรวจสอบฟีเจอร์เมื่อใดก็ตามที่เป็นไปได้ในการปรับปรุงรหัสบำรุงลดรหัสเปราะและลดความเสี่ยงของรหัสความแตกแยกในเหตุการณ์ของการอัปเดสตริงที่ UA ในอนาคต

สำหรับข้อมูลเพิ่มเติมให้ดู[สตริงตัวแทนผู้ใช้ Microsoft Edge (เดสก์ท็อป)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)