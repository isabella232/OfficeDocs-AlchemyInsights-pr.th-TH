---
title: การตั้งค่า SMTP for the Microsoft 365 mail service
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: e4d16a8d04b4d2fb4bfa8cf84308e29f2b499e0680f656cc239411d06e5b077c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900895"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>การตั้งค่า SMTP for the Microsoft 365 mail service

ต่อไปนี้เป็นการตั้งค่า SMTP ของบริการMicrosoft 365จดหมายของคุณ:

**เซิร์ฟเวอร์**: smtp.office365.com </br>
**พอร์ต**: 587 </br>
**การเข้ารหัสลับ**: STARTTLS (สนับสนุนเฉพาะเวอร์ชัน TLS 1.2 เท่านั้นในขณะนี้ โปรดตรวจสอบให้แน่ใจว่าแอปพลิเคชันหรืออุปกรณ์ของคุณสนับสนุน TLS 1.2) </br>
**ชื่อผู้ใช้**: Office 365ของคุณ (เช่น example@yourdomain.com) </br>
**รหัสผ่าน**: รหัสผ่านOffice 365ของคุณ </br>
**การรับรองความถูกต้อง**: ต้องระบุ </br>
**ขีดจํากัดการส่ง**: 10,000 อีเมลต่อวัน </br>

For POP and IMAP settings, see [POP, IMAP, and SMTP settings](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกในการส่งอีเมลโดยใช้ Microsoft 365 และขั้นตอน ให้ดู วิธีการตั้งค่า[อุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อ](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)ส่งอีเมลโดยใช้Microsoft 365หรือOffice 365