---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665851"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun

ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้
  
บางข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:
  
 **ไม่สามารถติดตั้งซอฟต์แวร์ได้ 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์พีซีในคอนโซลผู้ดูแลระบบ Intun อ่านเอกสารนี้สําหรับข้อมูลเพิ่มเติม
  
 **รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดสามารถเกิดขึ้นได้ในสถานการณ์ต่อไปนี้:
  
-  ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์ ตรวจสอบเอกสารเหล่านี้เพื่อ[นําอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "ผู้ใช้อาจเข้าร่วมอุปกรณ์ไปยังโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี" ตั้งค่าเป็นผู้ใช้ทั้งหมดหรือเลือก อ่าน[เอกสารนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)สําหรับข้อมูลเพิ่มเติม

-  อุปกรณ์ถูกลงทะเบียนโดยผู้ใช้อื่นแล้ว ถ้าเป็นกรณีนี้ ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intunen หรือ unenroll อุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง

-  อุปกรณ์เป็น Windows 10 หน้าแรก เฉพาะ Windows 10 Pro, การศึกษาและองค์กร SKU เท่านั้นที่สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure

ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
-  ใช้[Intunเน เว็บไซต์การแก้ไขปัญหา](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม

-  ตรวจทานเอกสารเหล่านี้สําหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและการแก้ปัญหาให้กับแต่ละ:[การแก้ไขปัญหาและการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[เรียนรู้วิธีลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun](https://docs.microsoft.com/intune/windows-enroll)
