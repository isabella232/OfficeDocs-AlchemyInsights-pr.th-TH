---
title: ลงชื่อเข้าใช้ Microsoft Edge ด้วยตนเอง
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
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678847"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>ลงชื่อเข้าใช้ Microsoft Edge ด้วยตนเอง

ถ้าผู้ใช้ไม่ได้ลงชื่อเข้าใช้โดยอัตโนมัติในระหว่างประสบการณ์การใช้งานครั้งแรกผู้ใช้สามารถลงชื่อเข้าใช้ด้วยตนเองผ่านการตั้งค่าของเบราว์เซอร์หรือการลอยตัวของข้อมูลประจำตัว เมื่อต้องการจัดการการลงชื่อเข้าใช้ให้ใช้นโยบายต่อไปนี้:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -เพื่อให้แน่ใจว่าผู้ใช้มีโปรไฟล์ที่ทำงานใน Microsoft Edge เสมอ
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -เมื่อต้องการจำกัดการลงชื่อเข้าใช้ในชุดของบัญชีผู้ใช้ที่เชื่อถือได้
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -เมื่อต้องการปิดใช้งานการลงชื่อเข้าใช้หรือการบังคับให้ผู้ใช้ลงชื่อเข้าใช้

