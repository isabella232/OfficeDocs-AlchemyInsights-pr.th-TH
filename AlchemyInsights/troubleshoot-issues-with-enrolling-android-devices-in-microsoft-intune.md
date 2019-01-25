---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493406"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune

ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้
  
ปัญหาทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:
  
 **อุปกรณ์ไม่เข้ารหัสลับข้อผิดพลาดในเว็บไซต์บริษัท:** รุ่นที่ใหม่กว่าของ Android โดยเฉพาะอย่างยิ่งโดยเริ่มต้น ด้วย v7.0 จำเป็นต้องมีรหัสผ่านการเริ่มต้นระบบเพื่อให้แน่ใจว่า อุปกรณ์ของคุณถูกเข้ารหัสลับทั้งหมด วิธีแก้ไขปัญหาทั่วไปมีการ เปิดใช้งาน pin เริ่มต้นระบบ หรือเข้ารหัสลับอุปกรณ์ได้อย่างสมบูรณ์ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)สำหรับข้อมูลเพิ่มเติม 
  
 **อุปกรณ์ไม่ผ่านการตรวจสอบ ด้วยบริการ Intune หรือแสดงเป็น "Unhealthy" ในคอนโซล admin Intune:** 4.4 บาง Samsung และอุปกรณ์ 5.5 อาจไม่ตรวจสอบถามการบริการ มี 3 วิธีด้วยกันปัญหานี้: 
  
1. เปิดตัวเว็บไซต์บริษัท Intune แอพลิเคชัน ซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติด้วยตนเอง
    
2. ปรับปรุงอุปกรณ์ Android 6.0 หรือสูงกว่า
    
3. ปิดใช้งานตัวจัดการสมาร์ท Samsung จากเว็บไซต์บริษัท Intune ในการจัดการ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)สำหรับรายละเอียดเพิ่มเติมในการตัดสินค้าจากคลังและการแก้ปัญหาเหล่านี้ 
    
 **ผู้ใช้สิทธิ์การใช้งานชนิดไม่ถูกต้อง**หรือ**ผู้ใช้ไม่รู้จักชื่อข้อผิดพลาด:** ผู้ใช้จำเป็นต้องมอบหมายให้ใบอนุญาต Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน: ศูนย์ดูแล Office หรือ Azure เว็บไซต์ 
  
ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)สำหรับข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาให้กับแต่ละรายการ 
    
3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll)
    

