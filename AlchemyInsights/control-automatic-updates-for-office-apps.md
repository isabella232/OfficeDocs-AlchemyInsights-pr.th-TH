---
title: ควบคุมการอัปเดตอัตโนมัติสำหรับแอป Office
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
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747795"
---
# <a name="control-automatic-updates-for-office-apps"></a>ควบคุมการอัปเดตอัตโนมัติสำหรับแอป Office

ตามค่าเริ่มต้นการอัปเดตสำหรับแอป Office จะได้รับการดาวน์โหลดโดยอัตโนมัติและนำไปใช้ในพื้นหลังโดยไม่มีการขัดจังหวะของผู้ใช้ อย่างไรก็ตามผู้ดูแลระบบสามารถควบคุมวิธีการนำการอัปเดตไปใช้ได้โดยใช้การตั้งค่าการอัปเดต Office อัปเดตการตั้งค่าอนุญาตให้ผู้ดูแลระบบเปิดใช้งานหรือปิดใช้งานการอัปเดตอัตโนมัติแสดงหรือซ่อนปุ่ม **อัปเด** ตทันทีใน Office ตั้งค่ากำหนดเวลาสิ้นสุดการอัปเดตและอื่นๆ สำหรับข้อมูลโดยละเอียดให้ดูที่:

- [การกำหนดค่าการตั้งค่าการอัปเดตสำหรับ Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [ไม่ได้เปิดใช้งานการอัปเดตอัตโนมัติสำหรับ Office](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [กำหนดวิธีที่ Office ได้รับการอัปเดตหลังจากติดตั้งแล้ว](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

เมื่อต้องการตรวจทานการตั้งค่าการอัปเดตที่มีอยู่กับเครื่องไคลเอ็นต์ให้ทำตามขั้นตอนต่อไปนี้:

1. เปิดตัวแก้ไขรีจิสทรีโดยไปที่**เริ่ม**  >  **เรียกใช้**  >  **regedit**
2. สลับไปยังตำแหน่งที่ตั้งต่อไปนี้และตรวจทานการตั้งค่าการอัปเดต Office:  
    a. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**หมายเหตุ:**  ถ้ามีการตั้งค่าคีย์ OfficeMgmtCOM คุณอาจเห็นข้อความ "การอัปเดตจะถูกจัดการโดยผู้ดูแลระบบของ**Office**คุณ" ใน  >  **Account**  >  การ**อัปเดต**office บัญชี office สำหรับข้อมูลเพิ่มเติมให้ดูที่ [จัดการการอัปเดตเป็นแอป microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า microsoft จุดสิ้น](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)สุด  