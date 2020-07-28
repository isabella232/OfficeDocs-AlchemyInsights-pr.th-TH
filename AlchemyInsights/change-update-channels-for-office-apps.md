---
title: เปลี่ยนช่องทางการปรับปรุงสําหรับแอป Office
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
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440023"
---
# <a name="change-update-channels-for-office-apps"></a>เปลี่ยนช่องทางการปรับปรุงสําหรับแอป Office

สําหรับการติดตั้ง Office ใหม่ ให้ใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ Office เพื่อเลือกช่องทางการปรับปรุงที่ต้องการ แล้วติดตั้งแอป Office (หรือติดตั้งใหม่) สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การจัดการการตั้งค่าการดาวน์โหลดซอฟต์แวร์ใน Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) 

**หมายเหตุ** ช่องการปรับปรุงที่เลือกโดยใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ Office นําไปใช้กับผู้ใช้ทั้งหมดที่ทําการติดตั้งใหม่โดยใช้พอร์ทัล O365 สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การดาวน์โหลดและติดตั้งหรือติดตั้ง Microsoft 365 หรือ Office 2019 ใหม่บนพีซีหรือ Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)   

สําหรับการติดตั้ง Office ที่มีอยู่ ให้ใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อสลับไปยังช่องทางการปรับปรุงที่แตกต่างกัน:  

1. ดาวน์โหลดรุ่นล่าสุดของเครื่องมือการปรับใช้ Office (setup.exe) จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)
2. ระบุชื่อของช่องสัญญาณที่คุณต้องการสลับไป สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตัวเลือกการตั้งค่าคอนฟิกสําหรับเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)
3. สร้างไฟล์ XML การกําหนดค่าที่ระบุ update.xmlชื่อช่องสัญญาณที่เหมาะสม  
    a. <Configuration>  
    b. <ช่องทางการปรับปรุง **="รายเดือน"** />  
    c. </Configuration>
4. จากพร้อมท์คําสั่งการยกระดับ สลับไปยังตําแหน่งที่ตั้งของโฟลเดอร์ที่setup.exeอยู่ และเรียกใช้คําสั่งต่อไปนี้:  
    a. setup.exe /กําหนดค่าupdate.xml
5. เริ่มต้นโปรแกรมประยุกต์ Office (เช่น Excel) แล้วเลือก**File**  >  **บัญชี**แฟ้ม ในส่วน ข้อมูลผลิตภัณฑ์ ให้เลือก**อัปเดตตัวเลือก**  >  **การปรับปรุงเดี๋ยวนี้**

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีการสลับช่องทางการปรับปรุงสําหรับ Office Apps ที่มีอยู่](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

สําหรับการสลับสถานีการปรับปรุงสําหรับผู้ใช้ที่เลือก หรือ โดยใช้ตัวจัดการการตั้งค่าคอนฟิก (SCCM), กําหนดค่าการตั้งค่าสถานีปรับปรุงโดยใช้วัตถุนโยบายกลุ่ม สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ภาพรวมของช่องทางการปรับปรุงสําหรับแอป Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy) สําหรับรายละเอียด ให้ดูที่[วิธีจัดการแชนเนล Office 365 ProPlus สําหรับผู้เชี่ยวชาญด้าน IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) [และจัดการการอัปเดตแอป Microsoft 365 ด้วยตัวจัดการการตั้งค่าคอนฟิกปลายทางของ Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)