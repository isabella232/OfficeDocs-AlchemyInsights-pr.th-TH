---
title: ลงชื่อเข้าใช้Microsoft Edgeด้วยตนเอง
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050785"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>ลงชื่อเข้าใช้Microsoft Edgeด้วยตนเอง

ถ้าผู้ใช้ไม่ลงชื่อเข้าใช้โดยอัตโนมัติระหว่างประสบการณ์การใช้งานครั้งแรก ผู้ใช้สามารถลงชื่อเข้าใช้ผ่านการตั้งค่าของเบราว์เซอร์หรือแถบเลื่อนข้อมูลเฉพาะตัวได้ด้วยตนเอง เมื่อต้องการจัดการการลงชื่อเข้าใช้ ให้ใช้นโยบายต่อไปนี้

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - เมื่อต้องการตรวจสอบให้แน่ใจว่าผู้ใช้มีโปรไฟล์งานในMicrosoft Edgeเสมอ
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - เมื่อต้องการจํากัดการลงชื่อเข้าใช้ชุดบัญชีที่เชื่อถือได้
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - เมื่อต้องการปิดใช้งานการลงชื่อเข้าใช้หรือบังคับให้ผู้ใช้ลงชื่อเข้าใช้

