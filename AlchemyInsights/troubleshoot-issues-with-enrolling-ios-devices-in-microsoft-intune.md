---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658458"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune

ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้ 
  
ข้อผิดพลาดทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:
  
- **ทุนอุปกรณ์ที่มาถึง** ผู้ใช้มีอุปกรณ์เพิ่มเติมที่ลงทะเบียนไว้เกินขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เมื่อต้องการ[เอาอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **บริการนี้ไม่ได้รับการสนับสนุน นโยบายไม่มีการลงทะเบียน:** Apple ดันแจ้งเตือนบริการ (APNS) ที่จำเป็นต้องมีการตั้งค่าคอนฟิก หรือต่ออายุ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)สำหรับคำแนะนำเกี่ยวกับวิธีการทำเช่นนั้น 
    
- **ไม่ถูกต้องชนิดลิขสิทธิ์ของผู้ใช้หรือชื่อผู้ใช้ที่ไม่รู้จัก:** ผู้ใช้อาจต้องการกำหนดใบอนุญาต Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน:[ศูนย์ดูแล Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[Azure เว็บไซต์](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาแต่ละ:[คำแนะนำในการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และการ[แก้ไขปัญหาเอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)
    

