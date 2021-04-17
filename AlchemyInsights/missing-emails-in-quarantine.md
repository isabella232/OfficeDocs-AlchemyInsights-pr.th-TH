---
title: อีเมลหายไปในการกักกัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831753"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลหายไปในการกักกัน"

ผู้ดูแลระบบสามารถดู [เผยแพร่ หรือลบข้อความเหล่านี้ได้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

เมื่อต้องการเปิดศูนย์&การปฏิบัติตามนโยบาย [https://protection.office.com](https://protection.office.com/) ให้ไปที่ เมื่อต้องการเปิดหน้า การกักกัน โดยตรง ให้ไปที่ [https://protection.office.com/quarantine](https://protection.office.com/quarantine)  

คุณสามารถค้นหาด้วยค่าต่อไปนี้  

- **ID ข้อความ**: ตัวระบุที่ไม่รหัสเฉพาะส่วนกลางของข้อความ ถ้าคุณเลือกข้อความในรายการ ค่า  **ID**  ข้อความจะปรากฏขึ้นในบานหน้าต่าง  **แถบปลิว**  รายละเอียด ที่ปรากฏขึ้น ผู้ดูแลระบบสามารถใช้การติดตาม [ข้อความเพื่อค้นหา](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) ข้อความและค่า ID ข้อความที่สอดคล้องกัน
- **ที่อยู่อีเมลผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งเดียว
- **ที่อยู่อีเมลผู้รับ**: ที่อยู่อีเมลของผู้รับเดียว
- **เรื่อง**: ใช้ชื่อเรื่องทั้งหมดของข้อความ การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก

หลังจากที่คุณใส่เกณฑ์การค้นหา ให้คลิกปุ่ม รีเฟรช ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **รีเฟรช** เพื่อกรองผลลัพธ์  

cmdlet ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในการกักกันคือ:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้จะมีไว้เฉพาะข้อความเท่านั้น ไม่ใช่ไฟล์มัลแวร์จาก ATP for SharePoint Online, OneDrive for Business หรือ Teams
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)