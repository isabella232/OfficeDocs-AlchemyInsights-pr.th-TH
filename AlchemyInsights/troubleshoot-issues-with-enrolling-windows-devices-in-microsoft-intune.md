---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนWindowsในMicrosoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981060"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนWindowsในMicrosoft Intune

ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ด้านล่างเพื่อแก้ไขปัญหาของคุณทันที
  
ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหามีดังนี้
  
 **ไม่สามารถติดตั้งซอฟต์แวร์ได้ 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์พีซีในคอนโซลผู้ดูแลระบบ Intun1 อีกครั้ง อ่านคู่มือนี้เพื่อดูข้อมูลเพิ่มเติม
  
 **รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นในสถานการณ์ต่อไปนี้:
  
-  ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้[เพื่อเอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)ออก[หรือเปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "ผู้ใช้อาจเข้าร่วมอุปกรณ์ไปยัง Azure AD" ถูกตั้งค่าเป็น "ไม่มี" Set it to all or select users. [อ่านคู่มือ](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)นี้เพื่อดูข้อมูลเพิ่มเติม

-  อุปกรณ์ได้รับการลงทะเบียนโดยผู้ใช้อื่นแล้ว ถ้าเป็นกรณีนี้ ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intuned หรือยกเลิกการลงทะเบียนอุปกรณ์ด้วยตนเองก่อนลองอีกครั้ง

-  อุปกรณ์ดังกล่าวWindows 10 Homeอยู่ เฉพาะWindows 10 Pro การศึกษา และ Enterprise SKUs เท่านั้นที่สามารถAzure Active Directoryได้

แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
-  ใช้ [พอร์ทัลการแก้ไขปัญหา Intun1](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม

-  ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและการแก้ไขปัญหาแต่ละรายการ:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)[และ การแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[เรียนรู้วิธีการลงทะเบียนWindowsใน Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)
