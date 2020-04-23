---
title: ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788901"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมายของผู้ใช้

**วิธีที่ 1 **

1. เข้าสู่ระบบพอร์ทัล Microsoft 365

2. ไปที่ **ผู้ใช้ > ผู้ใช้ที่ใช้งานอยู่** (หรือ **กลุ่ม > กล่องจดหมายที่แชร์** ถ้าคุณตั้งค่านี้ในกล่องจดหมายที่แชร์)

3. เลือกผู้ใช้ที่มีกล่องจดหมาย Microsoft Exchange

4. บนเมนูที่ลอยอยู่ทางด้านขวาให้ไปที่ **การตั้งค่าจดหมาย > การตอบกลับอัตโนมัติ** (ถ้าเป็นกล่องจดหมายที่แชร์ เพียงคลิก **การตอบกลับอัตโนมัติ** บนเมนูที่ลอยอยู่)

**วิธีที่ 2 **

1. เข้าสู่ระบบพอร์ทัลผู้ดูแลระบบ Microsoft 365 โดยใช้ข้อมูลประจําตัวของผู้ดูแล

2. ขยาย **ศูนย์การจัดการ** จากนั้นคลิก **Exchange**

3. คลิกรูปภาพที่มุมขวาบน แล้วคลิก **ผู้ใช้อื่น** จากนั้นเลือกกล่องจดหมายของผู้ใช้ที่คุณต้องการเปลี่ยนแปลง

4. ทางด้านซ้าย ให้เลือก **ตัวเลือก** แล้วคลิก **จัดระเบียบอีเมล**จากนั้นคลิก **การตอบกลับอัตโนมัติ**

**วิธีที่ 3 **

เรียกใช้ cmdlet ต่อไปนี้ใน Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ cmdlet นี้ โปรดดู [Set-Msolcompanysettings](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)
