---
title: ควบคุมการอัปเดตอัตโนมัติOfficeแอป
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929900"
---
# <a name="control-automatic-updates-for-office-apps"></a>ควบคุมการอัปเดตอัตโนมัติOfficeแอป

ตามค่าเริ่มต้น การอัปเดตของแอปOfficeจะถูกดาวน์โหลดโดยอัตโนมัติและจะถูกใช้งานในเบื้องหลังโดยไม่มีการขัดจังหวะการใดๆ ของผู้ใช้ อย่างไรก็ตาม ผู้ดูแลระบบสามารถควบคุมวิธีการปรับใช้การอัปเดตโดยใช้Office การตั้งค่าการอัปเดต การตั้งค่าการอัปเดตจะอนุญาตให้ผู้ดูแลระบบเปิดใช้งานหรือปิดใช้งานการอัปเดตอัตโนมัติ แสดงหรือซ่อนปุ่ม อัปเดตเดี๋ยวนี้Office ตั้งค่าวันสิ้นสุดการอัปเดต และอื่นๆ ดูข้อมูลโดยละเอียดที่:

- [กําหนดค่าการตั้งค่าการอัปเดตOffice](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [ไม่ได้เปิดใช้งานการอัปเดตOfficeโดยอัตโนมัติ](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [กําหนดOfficeวิธีการอัปเดตหลังจากติดตั้ง](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

เมื่อต้องการตรวจสอบการตั้งค่าการอัปเดตที่มีอยู่ที่ปรับใช้กับเครื่องไคลเอ็นต์ ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. เปิด Registry Editor โดยไปที่ **เริ่ม**  >  **เรียกใช้**  >  **regedit**
2. สลับไปยังสถานที่ต่อไปนี้และตรวจสอบการตั้งค่า Officeอัปเดต:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**หมายเหตุ**  ถ้าคีย์ OfficeMgmtCOM ถูกตั้งค่าไว้ คุณอาจเห็นข้อความ "การอัปเดตได้รับการจัดการโดยผู้ดูแลระบบของคุณ" **Office**  >  **บัญชีผู้ใช้**  >  **Officeอัปเดต** ต่างๆ ดูข้อมูลเพิ่มเติมได้ที่ จัดการ[การอัปเดตMicrosoft 365 Appsด้วยMicrosoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)  