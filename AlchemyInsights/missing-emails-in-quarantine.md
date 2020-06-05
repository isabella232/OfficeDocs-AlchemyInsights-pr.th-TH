---
title: อีเมลที่ขาดไปในเขตกักกัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569562"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลที่ขาดหายไปในเขตกักกัน"

ผู้ดูแลระบบสามารถดู[ปล่อย หรือลบข้อความเหล่านี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

เมื่อต้องการเปิดศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย ให้ไปที่ [https://protection.office.com](https://protection.office.com/) เมื่อต้องการเปิดหน้าการกักกันโดยตรง ให้ไปที่ [https://protection.office.com/quarantine](https://protection.office.com/quarantine)  

คุณสามารถค้นหาตามค่าต่อไปนี้:  

- **รหัสข้อความ**: ตัวระบุที่ไม่ซ้ํากันทั่วโลกของข้อความ ถ้าคุณเลือกข้อความในรายการ ค่า**ID ข้อความ****จะปรากฏขึ้นในบานหน้าต่างลอย**รายละเอียดที่ปรากฏขึ้น ผู้ดูแลระบบสามารถใช้[การติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)เพื่อค้นหาข้อความและค่ารหัสข้อความที่สอดคล้องกันได้
- **ที่อยู่อีเมลผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งรายเดียว
- **ที่อยู่อีเมลของผู้รับ**: ที่อยู่อีเมลของผู้รับรายเดียว
- **เรื่อง**: ใช้เรื่องทั้งหมดของข้อความ การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก

หลังจากที่คุณป้อนเกณฑ์การค้นหาแล้ว ให้คลิกปุ่ม ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **รีเฟรช**เพื่อกรองผลลัพธ์  

cmdlets ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในกักกันได้แก่:
- [ลบ-กักกัน](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [ส่งออก-กักกัน](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [รับ-กักกัน](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [การแสดงตัวอย่าง-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้สําหรับข้อความเท่านั้น ไม่ใช่แฟ้มมัลแวร์จาก ATP สําหรับ SharePoint Online, OneDrive สําหรับธุรกิจ หรือทีม
- [ปล่อย- กักกัน](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)