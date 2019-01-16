---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316976"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune

ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้ 
  
ข้อผิดพลาดทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:
  
 **ไม่สามารถติดตั้งซอฟต์แวร์ 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอนต์พีซีในคอนโซล Admin Intune อีกครั้ง ตรวจทานเอกสารนี้สำหรับข้อมูลเพิ่มเติม 
  
 **รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นได้ในสถานการณ์ต่อไปนี้: 
  
1. ผู้ใช้มีอุปกรณ์เพิ่มเติมที่ลงทะเบียนไว้เกินขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เมื่อต้องการ[เอาอุปกรณ์ออก](https://docs.microsoft.com/en-us/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
2. "ผู้ใช้อาจเข้าร่วมอุปกรณ์เพื่อโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี" ตั้งค่าทั้งหมด หรือเลือกผู้ใช้ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings)สำหรับข้อมูลเพิ่มเติม 
    
3. อุปกรณ์มีการลงทะเบียนแล้ว โดยผู้ใช้อื่น ถ้าเป็นกรณีนี้ เอาอุปกรณ์ออกจากคอนโซล Azure Intune หรืออุปกรณ์ที่ unenroll ด้วยตนเองก่อนที่จะลองอีกครั้ง
    
4. อุปกรณ์ดังกล่าว Windows 10 หน้าแรก เฉพาะ Windows 10 Pro การศึกษา และองค์กร Sku สามารถรวมไดเรกทอรีที่ใช้งานอยู่ของ Azure
    
ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:
  
1. ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม 
    
2. ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาแต่ละ:[คำแนะนำในการแก้ไขปัญหา](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)และการ[แก้ไขปัญหาเอกสาร](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll)
  

