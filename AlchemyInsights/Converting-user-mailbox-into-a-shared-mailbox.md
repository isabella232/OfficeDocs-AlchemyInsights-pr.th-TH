---
title: แปลงกล่องจดหมายของผู้ใช้ลงในกล่องจดหมายที่ใช้ร่วมกันได้อย่างไร
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496454"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>แปลงเป็นกล่องจดหมายของผู้ใช้ลงในกล่องจดหมายที่ใช้ร่วมกัน

คุณสามารถแปลงได้เฉพาะกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกันถ้าผู้ใช้มีสิทธิ์การใช้งานของการแลกเปลี่ยน หลังจากกล่องจดหมายจะถูกแปลง จะยังคงแสดงอยู่ในรายการผู้ใช้ที่ใช้งานอยู่ได้เนื่องจากรายการที่มีกล่องจดหมายที่ใช้ร่วมกัน อย่างไรก็ตาม กล่องจดหมายถูกแปลงจะแสดงขึ้นในรายการกล่องจดหมายที่ใช้ร่วมกันด้วย 
  
ถ้าคุณพยายามแปลงกล่องจดหมายในคอนโซลการดูแลอัตราแลกเปลี่ยน และการแปลงล้มเหลว ล้างแคชของเบราว์เซอร์และคุกกี้ของคุณ แล้วลองอีกครั้ง ถ้าจะยังคงทำงานไม่ได้ ลองแปลงกล่องจดหมายในเชลล์จัดการการแลกเปลี่ยน โดยการเรียกใช้คำสั่งต่อไปนี้:
  
```
Set-Mailbox -Type Shared
```

ข้อมูลการแปลงกล่องจดหมายเพิ่มเติมจะพร้อมใช้งานในการ[แปลงเป็นกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกัน](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox)
  
