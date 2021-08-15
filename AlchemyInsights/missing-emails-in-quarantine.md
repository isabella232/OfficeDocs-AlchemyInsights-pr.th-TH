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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026241"
---
# <a name="missing-emails-in-quarantine"></a>อีเมลหายไปในการกักกัน"

ผู้ดูแลระบบสามารถดู [เผยแพร่ หรือลบข้อความเหล่านี้ได้](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

เมื่อต้องการเปิดศูนย์&การปฏิบัติตามนโยบาย [https://protection.office.com](https://protection.office.com/) ให้ไปที่ เมื่อต้องการเปิดหน้า การกักกัน โดยตรง ให้ไปที่ [https://protection.office.com/quarantine](https://protection.office.com/quarantine)  

คุณสามารถค้นหาด้วยค่าต่อไปนี้  

- **ID ข้อความ**: ตัวระบุที่ไม่รหัสเฉพาะส่วนกลางของข้อความ ถ้าคุณเลือกข้อความในรายการ ค่า  **ID**  ข้อความจะปรากฏขึ้นในบานหน้าต่าง  **แถบปลิว**  รายละเอียด ที่ปรากฏขึ้น ผู้ดูแลระบบสามารถใช้การติดตาม [ข้อความเพื่อค้นหา](/microsoft-365/security/office-365-security/message-trace-scc) ข้อความและค่า ID ข้อความที่สอดคล้องกัน
- **ที่อยู่อีเมลผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งเดียว
- **ที่อยู่อีเมลผู้รับ**: ที่อยู่อีเมลของผู้รับเดียว
- **เรื่อง**: ใช้ชื่อเรื่องทั้งหมดของข้อความ การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก

หลังจากที่คุณใส่เกณฑ์การค้นหา ให้คลิกปุ่ม รีเฟรช ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **รีเฟรช** เพื่อกรองผลลัพธ์

cmdlet ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในการกักกันคือ:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [การกักกันแสดงตัวอย่าง :](/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้จะมีไว้เฉพาะข้อความเท่านั้น ไม่ใช่ไฟล์มัลแวร์จาก Microsoft Defender Office 365 for SharePoint Online, OneDrive for Business หรือ Teams
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)