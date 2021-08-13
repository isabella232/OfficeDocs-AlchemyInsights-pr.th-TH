---
title: ID กฎการเตรียมใช้งานโปรไฟล์ iOS 1029
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "322"
- "3100011"
ms.assetid: 14d30092-8cf5-4fe6-a2a3-8a337e96cb1c
ms.openlocfilehash: a52c98af0f5c5de3122bfc344029588234611da894994d719c95f6af78944405
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925724"
---
# <a name="ios-provisioning-profiles"></a>โปรไฟล์การเตรียมใช้งาน iOS

สายงานของ iOS ของ Apple ใช้แนวคิดของโปรไฟล์การเตรียมใช้งานที่ใช้เพื่อตรวจสอบความสมบูรณ์ของแอปพลิเคชันและบังคับใช้นโยบายที่กําหนดในโปรไฟล์ โปรไฟล์การเตรียมใช้งานเหล่านี้จะหมดอายุหลังจาก 12 เดือน ดังนั้น โปรไฟล์ใหม่จึงต้องเชื่อมโยงกับแอปที่ปรับใช้เพื่อให้แอปสามารถเรียกใช้ต่อไปได้
  
บทความต่อไปนี้อธิบายวิธีสร้างการเชื่อมโยงโปรไฟล์การเตรียมใช้งานใหม่กับแอป iOS LOB ที่ปรับใช้ผ่าน Intuned: ใช้โปรไฟล์การเตรียมใช้งานแอป iOS เพื่อป้องกันไม่ให้ [แอปของคุณหมดอายุ](https://docs.microsoft.com/intune/app-provisioning-profile-ios)
  