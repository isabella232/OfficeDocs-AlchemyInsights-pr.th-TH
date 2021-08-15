---
title: ส่งอีเมลผ่านMicrosoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024225"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>ตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมล

เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกและขั้นตอนของคุณ ให้ดู[วิธีการตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมลโดยใช้](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)Microsoft 365
  
ถ้าคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดการใช้งานได้เมื่อเร็วๆ นี้ ปัญหาที่พบบ่อยที่สุดคือ:

- **ข้อผิดพลาดที่เกี่ยวข้องกับการรับรองความถูกต้องขณะใช้การส่งไคลเอ็นต์การรับรองความถูกต้องของ SMTP** เราเพิ่งเปลี่ยนแปลงบางอย่างที่เกี่ยวข้องกับวิธีการใช้งานการรับรองความถูกต้องของ SMTP For more information about how to resolve issues, see the authentication unsuessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **เรายอมรับเฉพาะเวอร์ชัน TLS 1.2 ขณะที่สร้างการเชื่อมต่อที่ปลอดภัยOffice 365** ถ้าคุณใช้การเชื่อมต่อที่ปลอดภัย (TLS) ตรวจสอบให้แน่ใจว่าอุปกรณ์แอปพลิเคชันของคุณสนับสนุน TLS 1.2 For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
ดูปัญหาและวิธีแก้ปัญหาอื่นๆ[ที่แก้ไขปัญหาเกี่ยวกับเครื่องพิมพ์ สแกนเนอร์](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)และแอปพลิเคชัน LOB ที่ส่งอีเมลโดยใช้Microsoft 365 หรือOffice 365

เมื่อต้องการดูอุปกรณ์ที่ได้รับผลกระทบ ให้ไปที่รายงาน ไคลเอ็นต์ [การรับรองความถูกต้องของ](https://protection.office.com/mailflow/dashboard)SMTP

**หมายเหตุ**: Exchange Onlineสถานการณ์การส่งจดหมายเป็นกลุ่มไม่ได้ เมื่อต้องการส่งอีเมลเชิงพาณิชย์เป็นกลุ่ม (ตัวอย่างเช่น จดหมายข่าวของลูกค้า) คุณควรใช้ผู้ให้บริการของบริษัทอื่นที่มีข้อมูลไม่มากในบริการเหล่านี้
