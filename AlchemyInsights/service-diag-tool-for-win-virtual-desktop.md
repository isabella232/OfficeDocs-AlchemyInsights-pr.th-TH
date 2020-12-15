---
title: เครื่องมือการวินิจฉัยบริการสำหรับ Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680234"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>เครื่องมือการวินิจฉัยบริการสำหรับ Windows Virtual Desktop

Windows Virtual Desktop (WVD) มีเครื่องมือการวินิจฉัยที่ช่วยให้ผู้ดูแลระบบสามารถระบุข้อผิดพลาดผ่านทางส่วนติดต่อเดียว เครื่องมือนี้จะบันทึกข้อมูลที่เกี่ยวข้องกับการวินิจฉัยเมื่อใดก็ตามที่ WVD ถูกใช้งานโดยผู้ที่ได้รับมอบหมายบทบาท WVD แต่ละแฟ้มบันทึกจะมีข้อมูลเกี่ยวกับบทบาท WVD ที่เกี่ยวข้องกับกิจกรรมข้อความแสดงข้อผิดพลาดที่ปรากฏขึ้นในระหว่างเซสชันและข้อมูลเกี่ยวกับผู้เช่าและผู้ใช้ การวิเคราะห์บันทึกของ Azure สามารถกำหนดค่าให้จับภาพบันทึกกิจกรรมที่สร้างขึ้นโดยเครื่องมือการวินิจฉัยได้ โดยมีวิธีการดังต่อไปนี้:

1. สร้างเวิร์กสเปซการวิเคราะห์บันทึกที่มี[พอร์ทัล azure](https://go.microsoft.com/fwlink/?linkid=2129500)หรือ[azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [เชื่อมต่อคอมพิวเตอร์ที่มี Windows กับหน้าจอ Azure](https://go.microsoft.com/fwlink/?linkid=2129913) รับ ID ของเวิร์กสเปซและคีย์หลักของพื้นที่ทำงานของคุณ ตัวช่วยสร้างการตั้งค่าต้องการข้อมูลนี้เพื่อกำหนดค่าตัวแทนอย่างถูกต้องและตรวจสอบให้แน่ใจว่าสามารถสื่อสารกับหน้าจอ Azure ได้อย่างถูกต้อง
1. [ผลักดันข้อมูลการวินิจฉัยไปยังพื้นที่ทำงานของคุณ](https://go.microsoft.com/fwlink/?linkid=2128284) คุณสามารถผลักดันการวินิจฉัยข้อมูลจากผู้เช่า WVD ของคุณไปยังการวิเคราะห์บันทึกสำหรับพื้นที่ทำงานของคุณ
1. [ระบุและวินิจฉัยปัญหา](https://go.microsoft.com/fwlink/?linkid=2128338) ที่เกี่ยวข้องกับ WVD ภายในหรือภายนอก

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกำหนดค่าเครื่องมือการวินิจฉัยของบริการสำหรับ WVD ให้ดูที่[ใช้การวิเคราะห์บันทึกสำหรับฟีเจอร์การวินิจฉัย](https://go.microsoft.com/fwlink/?linkid=2128084)
