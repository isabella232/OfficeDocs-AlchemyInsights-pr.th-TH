---
title: แก้ไขปัญหาเกี่ยวกับอุปกรณ์ iOS ที่ลงทะเบียนใน Microsoft Intune
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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669267"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับอุปกรณ์ iOS ที่ลงทะเบียนใน Microsoft Intune

ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้ 
  
ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ไข:
  
- เข้า**ถึงฝาอุปกรณ์**แล้ว ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เพื่อ[เอาอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการการแจ้งเตือนแบบพุชของ Apple (apn) จำเป็นต้องได้รับการกำหนดค่าหรือต่ออายุ ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) เพื่อดูคำแนะนำเกี่ยวกับวิธีการทำงาน 
    
- **ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่รู้จักชื่อผู้ใช้ที่ไม่ถูกต้อง:** ผู้ใช้จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อมอบหมายสิทธิ์การใช้งานผ่าน:[ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณให้ทำดังนี้
  
1. ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละ[คำแนะนำการแก้ไข](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)ปัญหาและ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)
    

