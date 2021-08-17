---
title: Microsoft Defender Office 365 for SharePoint, OneDrive และ Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 0d0fff3e699d46af2a19a8ad60696b824bafa109
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314981"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender Office 365 for SharePoint, OneDrive และ Microsoft Teams

ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อเปิดใช้งาน Microsoft Defender Office 365:

1. ไปที่ [https://protection.office.com](https://protection.office.com) และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบความปลอดภัย

2. ในบานหน้าต่างนําทางด้านซ้าย ภายใต้ **การจัดการภัยคุกคาม** ให้เลือก **นโยบาย** \> **ตู้เซฟสิ่งที่แนบมา**

3. เลือก **เปิด Defender Office 365 SharePoint OneDrive และ Microsoft Teams**

4. [สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) เพื่อรับการแจ้งเตือนเมื่อเราตรวจพบไฟล์ที่เป็นอันตราย

ดูคําแนะ[นําทั้งหมดตู้เซฟ สิ่งที่แนบมาSharePoint OneDrive และ Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**หมายเหตุ**: ตามการออกแบบ Microsoft Defender for Office 365จะไม่สแกนทุกไฟล์ใน SharePoint Online, OneDrive for Business หรือ Microsoft Teams ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้กิจกรรมการแชร์ กิจกรรมของแขก และสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย For more information, see[ตู้เซฟ Attachments for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
