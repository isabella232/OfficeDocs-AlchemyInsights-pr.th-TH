---
title: เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: fb69bce40ab56b162c715af6a0647c8219c5564f
ms.sourcegitcommit: dab885f2cb99057e959fb9be334f5a3a26a64058
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2020
ms.locfileid: "46665481"
---
# <a name="change-update-channels-for-office-apps"></a>เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office

สำหรับการติดตั้ง Office ใหม่ให้ใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ของ Office เพื่อเลือกแชนเนลการอัปเดตที่ต้องการจากนั้นติดตั้ง (หรือติดตั้งใหม่) แอป Office สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการการตั้งค่าการดาวน์โหลดซอฟต์แวร์ใน Office ๓๖๕](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) 

**หมายเหตุ:** ช่องทางการอัปเดตที่เลือกโดยใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ของ Office จะนำไปใช้กับผู้ใช้ทุกคนที่ทำการติดตั้งใหม่โดยใช้ O365 portal สำหรับข้อมูลเพิ่มเติมให้ดูที่[ดาวน์โหลดและติดตั้งหรือติดตั้ง Microsoft ๓๖๕หรือ Office ๒๐๑๙อีกครั้งบนพีซีหรือ Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)   

สำหรับการติดตั้ง Office ที่มีอยู่ให้ใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อสลับไปยังแชนเนลการอัปเดตที่แตกต่างกันดังนี้  

1. ดาวน์โหลดเวอร์ชันล่าสุดของเครื่องมือการปรับใช้ Office (setup.exe) จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)
2. ระบุชื่อของแชนเนลที่คุณต้องการสลับไปใช้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตัวเลือกการกำหนดค่าสำหรับเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)
3. สร้างไฟล์ XML การกำหนดค่าที่ระบุชื่อแชนเนลที่เหมาะสมตัวอย่างเช่น update.xml  
    `<Configuration> 
    <Updates **Channel="Monthly"** />  
    </Configuration>`
4. จากพร้อมท์คำสั่งยกระดับให้สลับไปยังตำแหน่งที่ตั้งของโฟลเดอร์ที่ setup.exe อยู่และเรียกใช้คำสั่งต่อไปนี้:  
    a. setup.exe c:\odt\setup.exe/configure update.xml
5. เริ่มแอปพลิเคชัน Office (เช่น Excel) แล้วเลือก**File**  >  **บัญชีผู้ใช้**ไฟล์ ในส่วนข้อมูลผลิตภัณฑ์ให้เลือกอัปเดตตัว**เลือกการอัปเด**  >  **ตเดี๋ยวนี้**

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการสลับช่องทางการอัปเดตสำหรับแอป Office ที่มีอยู่](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

สำหรับการสลับช่องทางการอัปเดตสำหรับกลุ่มผู้ใช้ที่เลือกหรือโดยการใช้ตัวจัดการการตั้งค่าคอนฟิก (SCCM) ให้กำหนดค่าการตั้งค่าการอัปเดตระเบียนโดยใช้วัตถุนโยบายกลุ่ม สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ภาพรวมของช่องทางการอัปเดตสำหรับแอป Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy) สำหรับรายละเอียดให้ดู [ที่วิธีการจัดการ Office ๓๖๕ ProPlus channel สำหรับผู้เชี่ยวชาญด้าน it](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) และ [จัดการการอัปเดตเป็นแอป Microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า microsoft จุดสิ้น](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)สุด