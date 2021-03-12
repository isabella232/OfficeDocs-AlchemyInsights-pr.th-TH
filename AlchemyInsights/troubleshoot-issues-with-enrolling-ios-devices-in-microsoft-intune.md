---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708981"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun1

ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ในรายการด้านล่างเพื่อแก้ไขปัญหาของคุณทันที 
  
ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหาบางอย่าง มีดังนี้
  
- **ถึงจุดสูงสุดของอุปกรณ์แล้ว** ผู้ใช้ลงทะเบียนอุปกรณ์มากกว่าขีดจํากัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้ [เพื่อเอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe) ออก [หรือเปลี่ยนแปลงขีดจํากัด](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)ของอุปกรณ์
    
- **บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** Apple Push Notification Service (APNS) ต้องได้รับการกําหนดค่าหรือต่ออายุ ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) เพื่อดูคําแนะนําเกี่ยวกับวิธีแก้ไข 
    
- **ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้องหรือไม่รู้จักชื่อผู้ใช้:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน:[ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้ [พอร์ทัลการแก้ไขปัญหา Intuns](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและการแก้ปัญหา:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)[และการแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun1](https://docs.microsoft.com/intune/ios-enroll)
    

