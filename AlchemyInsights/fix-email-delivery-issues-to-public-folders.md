---
title: แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068831"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย

ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายของคุณ และผู้ส่งได้รับข้อผิดพลาด: ไม่พบ **(550 5.4.1)** ให้ยืนยันโดเมนอีเมลของโฟลเดอร์สาธารณะที่ถูกกําหนดค่าเป็น โดเมนรีเลย์ภายใน แทนที่จะเป็นโดเมนที่ใช้ทางการ

1. เปิด ศูนย์[Exchangeระบบ (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. ไปที่ **ลโฟล** \> **ว์จดหมายโดเมน** ที่ยอมรับ เลือกโดเมนที่ยอมรับ **แล้วคลิก** แก้ไข

3. ในหน้าคุณสมบัติที่เปิดขึ้น ถ้าชนิดของโดเมนถูกตั้งค่าเป็น ใช้ทางการ ให้เปลี่ยนค่าเป็น **รีเลย์** ภายใน **แล้วคลิก** บันทึก

ถ้าผู้ส่งภายนอกได้รับข้อผิดพลาดที่คุณไม่มีสิทธิ์ **(550 5.7.13)** ให้เรียกใช้สั่งต่อไปนี้ใน Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เพื่อดูสิทธิ์ของผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous. ตัวอย่างเช่น `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`
