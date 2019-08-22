---
title: แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525159"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย

ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะของคุณเปิดใช้งานจดหมาย และรายชื่อผู้ส่งที่ได้รับข้อผิดพลาด:**ไม่พบ (550 5.4.1)**, ตรวจสอบโดเมนอีเมลสำหรับโฟลเดอร์สาธารณะที่ถูกกำหนดค่าเป็นโดเมนรีเลย์ภายในที่แทน โดเมนที่เชื่อถือได้:

1. เปิด[ศูนย์ดูแล Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. **การรับส่งจดหมาย**ไป\>**โดเมน Accepted**เลือกโดเมนยอมรับได้ และจากนั้น คลิก**แก้ไข**

3. ในคุณสมบัติของหน้านั้นเปิด ถ้าชนิดโดเมนถูกตั้งค่าเป็น**Authoritative**เปลี่ยนค่าเป็น**สับเปลี่ยนภายใน**และจากนั้น คลิก**บันทึก**

หากผู้ส่งภายนอกได้รับการข้อผิดพลาด**คุณไม่ได้รับอนุญาต (550 5.7.13)**, เรียกใช้คำสั่งต่อไปนี้ใน[PowerShell ออนไลน์ของ Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เมื่อต้องการดูสิทธิ์สำหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกเพื่อส่งอีเมลไปที่โฟลเดอร์สาธารณะนี้ เพิ่มการเข้าถึง CreateItems ขวาไปผู้ใช้ที่ไม่ระบุชื่อ ตัวอย่างเช่น`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`
