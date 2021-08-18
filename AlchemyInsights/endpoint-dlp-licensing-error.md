---
title: ข้อผิดพลาดการให้สิทธิ์การใช้งาน DLP จุดสิ้นสุด
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090177"
---
# <a name="endpoint-dlp-licensing-error"></a>ข้อผิดพลาดการให้สิทธิ์การใช้งาน DLP จุดสิ้นสุด

เมื่อพยายามตั้งค่าจุดสิ้นสุด DLP ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้:

`Your organization is missing the licenses required to manage these devices`.

ตรวจสอบให้แน่ใจว่าคุณมีหนึ่งในการสมัครใช้งานหรือ Add-on ต่อไปนี้:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5การปฏิบัติตามข้อบังคับ
- Microsoft 365 A5การปฏิบัติตามนโยบาย
- Microsoft 365 E5และบรรษัทภิบาล
- Microsoft 365 A5การปกป้องข้อมูลและการกํากับดูแลข้อมูล

> [!NOTE]
> ซึ่งจะไม่ใช้งานกับการรวมสิทธิการใช้งานเช่น: Win E5 + O365 E5 + EMS E5 คุณต้องมีสิทธิ์การใช้งาน M365 E5 เท่านั้นในการตั้งค่าฟีเจอร์นี้

For more Endpoint DLP licensing information, see [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
