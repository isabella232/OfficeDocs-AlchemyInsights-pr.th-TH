---
title: ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมายของผู้ใช้
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506651"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>ตั้งค่าการตอบกลับอัตโนมัติสำหรับกล่องจดหมายของผู้ใช้

**วิธีที่ 1 **

1. ลงชื่อเข้าใช้พอร์ทัล Office 365

2. ไปที่ **ผู้ใช้ > ผู้ใช้ที่ใช้งานอยู่** (หรือ **กลุ่ม > กล่องจดหมายที่แชร์** ถ้าคุณตั้งค่านี้ในกล่องจดหมายที่แชร์)

3. เลือกผู้ใช้ที่มีกล่องจดหมาย Microsoft Exchange

4. บนเมนูที่ลอยอยู่ทางด้านขวาให้ไปที่ **การตั้งค่าจดหมาย > การตอบกลับอัตโนมัติ** (ถ้าเป็นกล่องจดหมายที่แชร์ เพียงคลิก **การตอบกลับอัตโนมัติ** บนเมนูที่ลอยอยู่)

**วิธีที่ 2 **

1. ลงชื่อเข้าใช้พอร์ทัลผู้ดูแลระบบ Office 365 โดยใช้ข้อมูลประจำตัวของผู้ดูแลระบบ

2. ขยาย **ศูนย์การจัดการ** จากนั้นคลิก **Exchange**

3. คลิกรูปภาพที่มุมขวาบน แล้วคลิก **ผู้ใช้อื่น** จากนั้นเลือกกล่องจดหมายของผู้ใช้ที่คุณต้องการเปลี่ยนแปลง

4. ทางด้านซ้าย ให้เลือก **ตัวเลือก** แล้วคลิก **จัดระเบียบอีเมล**จากนั้นคลิก **การตอบกลับอัตโนมัติ**

**วิธีที่ 3 **

เรียกใช้ cmdlet ต่อไปนี้ใน Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ cmdlet นี้ โปรดดู [Set-Msolcompanysettings](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)
