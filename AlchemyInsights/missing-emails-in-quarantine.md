---
title: อีเมลที่ขาดหายไปในการตรวจสอบสินค้า
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673733"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลที่ขาดหายไปในกักกัน "

ผู้ดูแลระบบสามารถ [ดูวางจำหน่ายหรือลบข้อความเหล่านี้ได้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

เมื่อต้องการเปิดศูนย์การปฏิบัติตามนโยบาย & ด้านความปลอดภัยให้ [https://protection.office.com](https://protection.office.com/) ไปที่ เมื่อต้องการเปิดหน้าการตรวจสอบสินค้าโดยตรงให้ [https://protection.office.com/quarantine](https://protection.office.com/quarantine) ไปที่  

คุณสามารถค้นหาโดยใช้ค่าต่อไปนี้:  

- **รหัสข้อความ**: ตัวระบุที่ไม่ซ้ำกันทั่วโลกของข้อความ ถ้าคุณเลือกข้อความในรายการค่า  **ID ข้อความ**  จะปรากฏขึ้นในบานหน้าต่างเมนูลอย  **รายละเอียด**  ที่ปรากฏขึ้น ผู้ดูแลระบบสามารถใช้การ [ติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) เพื่อค้นหาข้อความและค่า ID ข้อความที่สอดคล้องกันได้
- **ที่อยู่อีเมลของผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งรายเดียว
- **ที่อยู่อีเมลของผู้รับ**: ที่อยู่อีเมลของผู้รับรายเดียว
- **เรื่อง**: ใช้ทั้งชื่อเรื่องของข้อความ การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก

หลังจากที่คุณใส่เกณฑ์การค้นหาแล้วให้คลิกรีเฟรช ![ ปุ่มรี ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **เฟรช**เพื่อกรองผลลัพธ์  

Cmdlets ที่คุณใช้ในการดูและจัดการข้อความและไฟล์ในการกักกันได้แก่
- [ลบ-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [ส่งออก-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [รับ-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [ตัวอย่าง-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): โปรดสังเกตว่า cmdlet นี้มีไว้สำหรับข้อความเท่านั้นไม่ใช่ไฟล์มัลแวร์จาก ATP สำหรับ SharePoint Online, OneDrive for Business หรือทีม
- [การวางจำหน่าย-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)