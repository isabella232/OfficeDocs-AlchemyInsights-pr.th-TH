---
title: การแก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665851"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>การแก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ Windows ใน Microsoft Intune

ตรวจสอบแหล่งข้อมูลที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้
  
บางข้อความผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:
  
 **ซอฟต์แวร์ไม่สามารถติดตั้ง, 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์คอมพิวเตอร์อีกครั้งในคอนโซลการดูแล Intune ตรวจทานเอกสารฉบับนี้สำหรับข้อมูลเพิ่มเติม
  
 **รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดสามารถเกิดขึ้นได้ในสถานการณ์ต่อไปนี้:
  
-  ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เพื่อ[ลบอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "ผู้ใช้อาจเข้าร่วมอุปกรณ์กับโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี" ตั้งค่าให้ทั้งหมดหรือเลือกผู้ใช้ ตรวจทาน[เอกสารประกอบนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)สำหรับข้อมูลเพิ่มเติม

-  อุปกรณ์ได้ลงทะเบียนโดยผู้ใช้รายอื่นแล้ว ถ้าเป็นกรณีนี้ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intune หรือยกเลิกการลงทะเบียนอุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง

-  อุปกรณ์คือ Windows 10 Home เฉพาะ Windows 10 Pro, การศึกษาและองค์กร Sku สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure

แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
-  ใช้การ[แก้ปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม

-  ตรวจทานเอกสารเหล่านี้สำหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและแก้ปัญหาสำหรับแต่ละ[คำแนะนำการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)และ[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)
