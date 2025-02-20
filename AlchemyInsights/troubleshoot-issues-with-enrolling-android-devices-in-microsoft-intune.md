---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008097"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android Microsoft Intune

ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ด้านล่างเพื่อแก้ไขปัญหาของคุณทันที
  
ปัญหาและขั้นตอนการแก้ปัญหาทั่วไปบางขั้นตอน มีดังนี้
  
 **ข้อผิดพลาดอุปกรณ์ไม่ได้รับการเข้ารหัสลับในCompany Portal:** Android เวอร์ชันที่ใหม่กว่า โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับอย่างสมบูรณ์ โซลูชันทั่วไปคือการเปิดใช้งาน PIN เริ่มต้นหรือเข้ารหัสลับอุปกรณ์อย่างสมบูรณ์ ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) นี้เพื่อดูข้อมูลเพิ่มเติม
  
 **อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intun1 หรือแสดงเป็น "ไม่ร้อน" ในคอนโซลผู้ดูแลระบบ Intun1:** อุปกรณ์ Samsung 4.4 และ 5.5 บางรุ่นอาจไม่อยู่ในบริการ มี 3 วิธีที่เป็นไปได้ในการแก้ไขปัญหานี้:
  
1. เปิดแอปIntune Company Portalด้วยตนเอง ซึ่งจะเริ่มต้นการซิงค์อุปกรณ์โดยอัตโนมัติ

2. อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า

3. ปิดใช้งาน Samsung Smart Manager จากการจัดการIntune Company Portalของคุณ ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) เพื่อดูรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและการแก้ไขปัญหาเหล่านี้

 **ชนิดของสิทธิ์การใช้งานของผู้ใช้****ไม่ถูกต้อง หรือ ชื่อผู้ใช้ไม่รู้จัก ข้อผิดพลาด:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: Officeหรือพอร์ทัล Azure
  
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้ [พอร์ทัลการแก้ไขปัญหา Intun1](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม

2. ตรวจทาน [เอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) นี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้ลงทะเบียนและแก้ไขปัญหาในแต่ละรายการ

3. [เรียนรู้วิธีลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)
