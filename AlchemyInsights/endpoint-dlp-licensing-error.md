---
title: ข้อผิดพลาดการให้สิทธิ์การใช้งาน DLP
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564871"
---
# <a name="endpoint-dlp-licensing-error"></a>ข้อผิดพลาดการให้สิทธิ์การใช้งาน DLP

เมื่อพยายามตั้งค่าจุดสิ้นสุด DLP ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้:

`Your organization is missing the licenses required to manage these devices`.

ตรวจสอบให้แน่ใจว่าคุณมีหนึ่งในการสมัครใช้งานหรือ add-on ต่อไปนี้:

- Microsoft ๓๖๕ E5
- Microsoft ๓๖๕ A5 (EDU)
- การปฏิบัติตามกฎระเบียบของ Microsoft ๓๖๕ E5
- การปฏิบัติตามข้อกำหนดของ Microsoft ๓๖๕ A5
- Microsoft ๓๖๕ E5 การป้องกันและการกำกับดูแลข้อมูล
- Microsoft ๓๖๕ A5 protection และการกำกับดูแลข้อมูล

> [!NOTE]
> การดำเนินการนี้จะไม่ทำงานสำหรับการรวมสิทธิ์การใช้งานเช่น: Win + O365 E5 + EMS E5 คุณต้องมีสิทธิ์การใช้งาน M365 E5 ที่แท้จริงในการตั้งค่าฟีเจอร์นี้

สำหรับข้อมูลสิทธิ์การใช้งาน DLP ข้อมูลเพิ่มเติมให้ดู [ที่สิทธิ์การใช้งาน dlp ของจุดสิ้นสุด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
