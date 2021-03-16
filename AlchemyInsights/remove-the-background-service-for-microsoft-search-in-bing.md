---
title: เอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก
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
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816340"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>เอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก

เมื่อต้องการเอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก คุณสามารถลองวิธีแก้ไขต่อไปนี้:

1. เมื่อต้องการย้อนกลับไปยังการตั้งค่าโปรแกรมค้นหาดั้งเดิม ให้ทต่อไปนี้:

    a. สลับ **ปุ่มปิดใช้ Bing เป็น [เครื่องมือค้นหาเริ่มต้น](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)** ของคุณ

    b. [ไปที่ศูนย์การจัดการ Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) และล้างการตั้งค่าที่มีผลต่อผู้ใช้ทุกคนในองค์กรของคุณ

2. เมื่อต้องการเอาบริการพื้นหลังออกจากอุปกรณ์แต่ละเครื่อง ให้งานต่อไปนี้

    a. เลือก **แผงควบคุม >โปรแกรม>และฟีเจอร์**

    b. คลิกขวาที่ **Microsoft Search ใน Bing** ภายใต้รายการโปรแกรมที่ติดตั้ง **แล้วคลิก** ถอนการติดตั้ง

3. เมื่อต้องการเอาบริการพื้นหลังออกจากอุปกรณ์หลายเครื่องในองค์กรของคุณ ให้เข้าสู่ระบบในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในสคริปต์: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
