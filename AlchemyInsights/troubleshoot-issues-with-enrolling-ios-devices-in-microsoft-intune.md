---
title: แก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507022"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ iOS ใน Microsoft Intune

ตรวจสอบแหล่งข้อมูลที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้ 
  
บางข้อความผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:
  
- **ถึงฝาอุปกรณ์**แล้ว ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เพื่อ[ลบอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการแจ้งเตือนแบบพุชของ Apple (APNS) จำเป็นต้องมีการกำหนดค่าหรือต่ออายุ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)เพื่อดูคำแนะนำในการดำเนินการดังกล่าว 
    
- **ประเภทใบอนุญาตของผู้ใช้ไม่ถูกต้องหรือชื่อผู้ใช้ที่ไม่ได้**รับการยอมรับ: ผู้ใช้จำเป็นต้องได้รับใบอนุญาต Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน:[ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[เว็บไซต์ Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้การ[แก้ปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้สำหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและแก้ปัญหาสำหรับแต่ละ[คำแนะนำการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และ[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)
    

