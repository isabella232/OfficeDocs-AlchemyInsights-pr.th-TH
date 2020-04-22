---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759639"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune

ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้
  
ปัญหาทั่วไปและขั้นตอนการแก้ปัญหา:
  
 **ข้อผิดพลาดที่เข้ารหัสลับอุปกรณ์ในพอร์ทัลของบริษัท:** เวอร์ชันใหม่ของ Android โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณมีการเข้ารหัสอย่างเต็มที่ โซลูชันทั่วไปคือการเปิดใช้งาน pin เริ่มต้นระบบ หรือเข้ารหัสลับอุปกรณ์ทั้งหมด ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)สําหรับข้อมูลเพิ่มเติม
  
 **อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intune หรือแสดงเป็น "ไม่แข็งแรง" ในคอนโซลผู้ดูแลระบบ Intune:** อุปกรณ์บางตัวของ Samsung 4.4 และ 5.5 อาจไม่เช็คอินบริการ มี 3 วิธีแก้ไขปัญหาที่เป็นไปได้สําหรับปัญหานี้:
  
1. เปิดแอปเว็บไซต์ของบริษัท Intune ด้วยตนเอง ซึ่งจะเริ่มต้นการซิงค์อุปกรณ์โดยอัตโนมัติ

2. อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า

3. ปิดใช้งานตัวจัดการสมาร์ทของ Samsung จากการจัดการเว็บไซต์บริษัท Intune ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ปัญหาเหล่านี้

 **ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้อง**หรือ**ชื่อผู้ใช้ที่ไม่รู้จักข้อผิดพลาด:** ผู้ใช้จําเป็นต้องกําหนดสิทธิ์การใช้งาน Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure
  
ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ปัญหาของคุณ:
  
1. ใช้[การแก้ไขปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม

2. ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)เพื่อดูรายการของข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและวิธีแก้ปัญหาในแต่ละรายการ

3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์แอนดรอยด์ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)
