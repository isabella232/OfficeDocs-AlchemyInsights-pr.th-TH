---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658897"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune

ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้
  
ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ไข:
  
 **ไม่สามารถติดตั้งซอฟต์แวร์ได้ 0x80cf4017:** ใบรับรองบัญชีผู้ใช้ของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์ของพีซีในคอนโซลผู้ดูแลระบบ Intune อีกครั้ง ตรวจทานเอกสารนี้สำหรับข้อมูลเพิ่มเติม
  
 **รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นในสถานการณ์ต่อไปนี้:
  
-  ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เพื่อ[เอาอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "ผู้ใช้อาจเข้าร่วมอุปกรณ์ใน Azure AD" ถูกตั้งค่าเป็น "ไม่มี" ตั้งค่าเป็นทั้งหมดหรือเลือกผู้ใช้ ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) สำหรับข้อมูลเพิ่มเติม

-  อุปกรณ์ได้ลงทะเบียนโดยผู้ใช้อื่นแล้ว ถ้าเป็นกรณีนี้ให้เอาอุปกรณ์ออกจากคอนโซล Intune ของ Azure หรือการ unenroll อุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง

-  อุปกรณ์คือ Windows 10 Home เฉพาะ Windows 10 Pro, การศึกษาและ Sku ขององค์กรเท่านั้นที่สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure ได้

แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณให้ทำดังนี้
  
-  ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม

-  ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละ[คำแนะนำการแก้ไข](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)ปัญหาและ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)
