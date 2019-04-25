---
title: แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401461"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย

ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะของคุณเปิดใช้งานจดหมาย และรายชื่อผู้ส่งที่ได้รับข้อผิดพลาด:**ไม่พบ (550 5.4.1)**, ตรวจสอบโดเมนอีเมลสำหรับโฟลเดอร์สาธารณะที่ถูกกำหนดค่าเป็นโดเมนรีเลย์ภายในที่แทน โดเมนที่เชื่อถือได้:

1. เปิด[ศูนย์ดูแล Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. **การรับส่งจดหมาย**ไป\>**โดเมน Accepted**เลือกโดเมนยอมรับได้ และจากนั้น คลิก**แก้ไข**

3. ในคุณสมบัติของหน้านั้นเปิด ถ้าชนิดโดเมนถูกตั้งค่าเป็น**Authoritative**เปลี่ยนค่าเป็น**สับเปลี่ยนภายใน**และจากนั้น คลิก**บันทึก**

หากผู้ส่งภายนอกได้รับการข้อผิดพลาด**คุณไม่ได้รับอนุญาต (550 5.7.13)**, เรียกใช้คำสั่งต่อไปนี้ใน[PowerShell ออนไลน์ของ Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เมื่อต้องการดูสิทธิ์สำหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกเพื่อส่งอีเมลไปที่โฟลเดอร์สาธารณะนี้ เพิ่มการเข้าถึง CreateItems ขวาไปผู้ใช้ที่ไม่ระบุชื่อ ตัวอย่างเช่น`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`
