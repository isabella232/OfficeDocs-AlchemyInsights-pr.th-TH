---
title: แก้ไขปัญหาการนำส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677947"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>แก้ไขปัญหาการนำส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย

ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายของคุณได้และผู้ส่งได้รับข้อผิดพลาด: ไม่ **พบ (๕๕๐ 5.4.1)** ตรวจสอบโดเมนอีเมลสำหรับโฟลเดอร์สาธารณะที่ได้รับการกำหนดค่าเป็นโดเมน relay ภายในแทนที่จะเป็นโดเมนที่มีสิทธิ์:

1. เปิด[ศูนย์การจัดการ Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. ไปที่**Mail flow** \> **โดเมนที่ยอมรับ**จดหมายเวียนให้เลือกโดเมนที่ยอมรับแล้วคลิก**แก้ไข**

3. ในหน้าคุณสมบัติที่เปิดขึ้นถ้ามีการตั้งค่าชนิดโดเมนเป็น**สิทธิ์**ให้เปลี่ยนค่าเป็น**รีเลย์ภายใน**แล้วคลิก**บันทึก**

ถ้าผู้ส่งภายนอกได้รับข้อผิดพลาดที่ **คุณไม่มีสิทธิ์ (๕๕๐ 5.7.13)** ให้เรียกใช้คำสั่งต่อไปนี้ใน [PowerShell Online Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) เพื่อดูสิทธิ์สำหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` ตัว `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` อย่างเช่น

เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกส่งอีเมลไปยังโฟลเดอร์สาธารณะนี้ให้เพิ่มการเข้าถึง CreateItems ขวาไปยังผู้ใช้ที่ไม่ระบุชื่อ ตัว `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` อย่างเช่น
