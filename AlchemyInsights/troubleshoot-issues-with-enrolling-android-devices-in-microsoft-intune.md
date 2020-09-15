---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689973"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune

ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้
  
ปัญหาทั่วไปและขั้นตอนการแก้ไขปัญหาบางอย่าง:
  
 **ไม่มีข้อผิดพลาดในการเข้ารหัสลับอุปกรณ์ในพอร์ทัลของบริษัท:** เวอร์ชันที่ใหม่กว่าของ Android โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v 7.0 จำเป็นต้องใช้รหัสผ่านเริ่มต้นเพื่อตรวจสอบให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับทั้งหมดแล้ว วิธีแก้ไขปัญหาทั่วไปคือการเปิดใช้งาน pin เริ่มต้นระบบหรือเข้ารหัสลับอุปกรณ์ทั้งหมด ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) สำหรับข้อมูลเพิ่มเติม
  
 **อุปกรณ์ล้มเหลวในการเช็คอินด้วยบริการ Intune หรือแสดงเป็น "ไม่แข็งแรง" ในคอนโซลผู้ดูแลระบบ Intune:** อุปกรณ์ Samsung ๔.๔และ๕.๕บางรายการอาจไม่สามารถตรวจสอบได้ในบริการ มีวิธีแก้ไขปัญหาที่เป็นไปได้3วิธีดังนี้
  
1. เปิดแอป Intune ของพอร์ทัลของบริษัท Intune ด้วยตนเองซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติ

2. อัปเดตอุปกรณ์ไปยัง Android ๖.๐หรือสูงกว่า

3. ปิดใช้งานตัวจัดการสมาร์ทโฟนของ Samsung จากการจัดการพอร์ทัลบริษัท Intune ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ไขปัญหาเหล่านี้

 **ชนิดสิทธิ์การใช้งานของผู้ใช้****ไม่ได้รับการยอมรับข้อผิดพลาด:** ผู้ใช้ที่จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อมอบหมายสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure
  
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณให้ทำดังนี้
  
1. ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม

2. ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละรายการ

3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)
