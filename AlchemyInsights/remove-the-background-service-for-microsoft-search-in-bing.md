---
title: เอาบริการเบื้องหลังออกMicrosoft Searchอยู่ในBing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 07d24290fc3b13cce7a931c4cff15176c080b4413489ba1935b6886939ea3874
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53982392"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>เอาบริการเบื้องหลังออกMicrosoft Searchอยู่ในBing

เมื่อต้องการเอาบริการพื้นหลังMicrosoft Searchใน Bingลองวิธีแก้ไขต่อไปนี้:

1. เมื่อต้องการย้อนกลับไปยังการตั้งค่าเดิมของเครื่องมือค้นหา ให้ทต่อไปนี้:

    a. สลับ **ปุ่มBingโปรแกรมค้นหา [เริ่มต้นของคุณ](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)สลับ** เป็น ปิด

    b. [ไปที่ศูนย์การจัดการ Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)และล้างการตั้งค่าที่มีผลต่อผู้ใช้ทุกคนในองค์กรของคุณ

2. เมื่อต้องการเอาบริการเบื้องหลังออกจากอุปกรณ์แต่ละเครื่อง ให้เริ่มการงานต่อไปนี้

    a. เลือก **แผงควบคุม >โปรแกรม>และฟีเจอร์**

    b. คลิกขวา **Microsoft Searchใน Bing** ภายใต้รายการโปรแกรมที่ติดตั้ง **แล้วคลิก** ถอนการติดตั้ง

3. เมื่อต้องการเอาบริการพื้นหลังออกจากอุปกรณ์หลายเครื่องในองค์กรของคุณ ให้เข้าสู่ระบบในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในสคริปต์: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
