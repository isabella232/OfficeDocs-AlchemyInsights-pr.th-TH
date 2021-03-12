---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709017"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1

ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ในรายการด้านล่างเพื่อแก้ไขปัญหาของคุณทันที
  
ปัญหาทั่วไปและขั้นตอนการแก้ปัญหาบางอย่าง:
  
 **ข้อผิดพลาดอุปกรณ์ไม่เข้ารหัสลับในพอร์ทัลของบริษัท:** Android เวอร์ชันที่ใหม่กว่า โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับอย่างสมบูรณ์ วิธีแก้ไขปัญหาทั่วไปคือการเปิดใช้งาน PIN การเริ่มต้นหรือการเข้ารหัสลับอุปกรณ์อย่างสมบูรณ์ ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) นี้เพื่อดูข้อมูลเพิ่มเติม
  
 **อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intun1 หรือแสดงเป็น "ไม่healthy" ในคอนโซลผู้ดูแลระบบ Intun1:** อุปกรณ์ Samsung 4.4 และ 5.5 บางเครื่องอาจไม่ตรวจสอบบริการ มีวิธีแก้ไขปัญหาที่เป็นไปได้ 3 วิธี:
  
1. เปิดแอป Intun1 Company Portal ด้วยตนเอง ซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติ

2. อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า

3. ปิดใช้งาน Samsung Smart Manager จากการจัดการ Intun1 Company Portal ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) เพื่อดูรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและการแก้ไขปัญหาเหล่านี้

 **ข้อผิดพลาดชนิดสิทธิ์การใช้งาน****ของผู้ใช้ไม่ถูกต้องหรือไม่รู้จักชื่อผู้ใช้:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure
  
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้ [พอร์ทัลการแก้ไขปัญหา Intuns](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม

2. ตรวจทาน [เอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) นี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้ลงทะเบียนและแก้ไขปัญหาในแต่ละรายการ

3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1](https://docs.microsoft.com/intune/android-enroll)
