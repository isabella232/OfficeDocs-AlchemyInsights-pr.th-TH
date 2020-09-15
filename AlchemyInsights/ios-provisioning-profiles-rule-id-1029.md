---
title: โปรไฟล์การเตรียมใช้งานโปรไฟล์ของ iOS รหัส๑๐๒๙
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
ms.openlocfilehash: a571261ffcb327da50832bc5cb7169b769c2122c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695812"
---
# <a name="ios-provisioning-profiles"></a>โปรไฟล์การเตรียมใช้งาน iOS

Apple iOS line-ของธุรกิจใช้แนวคิดของโปรไฟล์การเตรียมใช้งานที่ใช้ในการตรวจสอบความถูกต้องของความสมบูรณ์ของแอปพลิเคชันและบังคับใช้นโยบายที่กำหนดไว้ในโปรไฟล์ โปรไฟล์การเตรียมใช้งานเหล่านี้จะหมดอายุหลังจาก12เดือนและดังนั้นโปรไฟล์ใหม่จะต้องเชื่อมโยงกับแอปที่ปรับใช้เพื่อให้แอปสามารถทำงานต่อไป
  
บทความต่อไปนี้จะอธิบายวิธีการสร้างการเชื่อมโยงโปรไฟล์การเตรียมใช้งานใหม่กับแอป iOS LOB ที่จัดวางผ่าน Intune: [ใช้โปรไฟล์การเตรียมใช้งานแอป ios เพื่อป้องกันไม่ให้แอปของคุณหมดอายุ](https://docs.microsoft.com/intune/app-provisioning-profile-ios)
  