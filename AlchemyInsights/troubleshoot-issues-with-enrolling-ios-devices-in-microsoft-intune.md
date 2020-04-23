---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736177"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune

ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้ 
  
ข้อความแสดงข้อผิดพลาดและขั้นตอนการแก้ปัญหาที่พบบ่อย:
  
- **ถึงอุปกรณ์แล้ว** ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์ ตรวจสอบเอกสารเหล่านี้เพื่อ[เอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)ออก หรือ[เปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการแจ้งเตือนแบบพุชของ Apple (APNS) จําเป็นต้องได้รับการกําหนดค่าหรือต่ออายุ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)สําหรับคําแนะนําเกี่ยวกับวิธีการทําเช่นนั้น 
    
- **ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้องหรือชื่อผู้ใช้ที่ไม่รู้จัก:** ผู้ใช้จําเป็นต้องได้รับใบอนุญาต Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน[: ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือพอร์ทัล[Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ปัญหาของคุณ:
  
1. ใช้[การแก้ไขปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้เพื่อดูรายการของข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและวิธีแก้ปัญหาแต่ละรายการ:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [เรียนรู้วิธีลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)
    

