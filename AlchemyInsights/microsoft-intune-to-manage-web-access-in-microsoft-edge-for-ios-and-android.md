---
title: ใช้ Microsoft Intune ในการจัดการการเข้าถึงเว็บใน Microsoft Edge สำหรับ iOS และ Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679610"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a>ใช้ Microsoft Intune ในการจัดการการเข้าถึงเว็บใน Microsoft Edge สำหรับ iOS และ Android

Microsoft Edge for iOS และ Android ช่วยให้ผู้ใช้สามารถเรียกดูเว็บจากหลายโปรไฟล์ที่แยกจากกันได้อย่างสมบูรณ์

ความสามารถในการป้องกันที่ดีที่สุดสำหรับข้อมูล Microsoft ๓๖๕จะพร้อมใช้งานเมื่อคุณสมัครใช้งาน office Mobility + ชุดการรักษาความปลอดภัยซึ่งรวมถึง Microsoft Intune และ Azure Active Directory Premium เช่นการเข้าถึงแบบมีเงื่อนไข อย่างน้อยที่สุดคุณจะต้องปรับใช้นโยบายการเข้าถึงตามเงื่อนไขที่ (1) ช่วยให้ผู้ใช้เชื่อมต่อจากอุปกรณ์เคลื่อนที่ไปยัง Microsoft Edge สำหรับ iOS และ Android และ (2) ใช้นโยบายการป้องกันแอป Microsoft Intune ที่มีประสบการณ์การใช้งานการป้องกันที่ได้รับการป้องกัน

เมื่อต้องการทำความเข้าใจวิธีที่คุณสามารถใช้การเข้าถึงแบบมีเงื่อนไขและนโยบายให้ดู:

[นำนโยบายการเข้าถึงแบบมีเงื่อนไขของ Azure Active Directory ไปใช้](https://go.microsoft.com/fwlink/?linkid=2132481)

[สร้างนโยบายการป้องกันแอป Microsoft Intune](https://go.microsoft.com/fwlink/?linkid=2132651)

[ใช้การลงชื่อเข้าใช้ครั้งเดียวสำหรับ Azure Active Directory –แอปเว็บที่เชื่อมต่ออยู่ในเบราว์เซอร์ที่มีการป้องกันด้วยนโยบาย](https://go.microsoft.com/fwlink/?linkid=2132482)

[ใช้การกำหนดค่าแอปเพื่อจัดการประสบการณ์การใช้งานการเรียกดู](https://go.microsoft.com/fwlink/?linkid=2132483)

[อนุญาตให้ใช้บัญชีที่ทำงานและที่โรงเรียนเท่านั้น](https://go.microsoft.com/fwlink/?linkid=2132652)

[ปรับใช้นโยบายการกำหนดค่าทั่วไปของแอป](https://go.microsoft.com/fwlink/?linkid=2132653)

[การปรับใช้นโยบายการกำหนดค่าแอปสำหรับการป้องกันข้อมูล](https://go.microsoft.com/fwlink/?linkid=2132654)

[ใช้ตัวจัดการจุดสิ้นสุดของ Microsoft เพื่อปรับใช้นโยบายการกำหนดค่าแอป](https://go.microsoft.com/fwlink/?linkid=2132707)

เมื่อต้องการเรียนรู้วิธีการเข้าถึงบันทึกของแอปที่ได้รับการจัดการให้ดู[ที่ใช้ Microsoft Edge สำหรับ iOS และ Android เพื่อเข้าถึงบันทึกของแอปที่มีการจัดการ](https://go.microsoft.com/fwlink/?linkid=2132578)
