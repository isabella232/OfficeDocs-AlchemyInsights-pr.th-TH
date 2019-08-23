---
title: นโยบายการเก็บข้อมูลในศูนย์ดูแล Exchange ไม่ทำงาน
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551362"
---
# <a name="retention-policies-in-exchange-admin-center"></a>นโยบายการเก็บข้อมูลในศูนย์ดูแลอัตราแลกเปลี่ยน

 **ปัญหา:** สร้างใหม่ หรือนโยบายการเก็บข้อมูลที่ปรับปรุงแล้วในศูนย์ดูแล Exchange จะไม่นำไปใช้กับกล่องจดหมาย หรือรายการถูกย้ายไปยังกล่องจดหมายการเก็บถาวร หรือถูกลบ 
  
 **สาเหตุราก:**
  
- ซึ่งอาจเนื่องมาจากผู้**จัดการผู้ช่วยของโฟลเดอร์**ยังไม่ประมวลผลกล่องจดหมายของผู้ใช้ ผู้จัดการโฟลเดอร์ช่วยพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรของคุณใช้ cloud ทุก ๆ 7 วันครั้งเดียว ถ้าคุณเปลี่ยนแปลงแท็กเก็บข้อมูล หรือใช้นโยบายการเก็บข้อมูลที่แตกต่างกันไปยังกล่องจดหมาย คุณสามารถรอจนกระทั่งการจัดการโฟลเดอร์ช่วยประมวลผลกล่องจดหมาย หรือคุณสามารถเรียกใช้ cmdlet ManagedFolderAssistant เริ่มต้นเพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยในการประมวลผลเฉพาะ กล่องจดหมาย เรียกใช้ cmdlet นี้จะเป็นประโยชน์สำหรับการทดสอบ หรือการแก้ไขปัญหานโยบายการเก็บข้อมูลหรือการตั้งค่าแท็กการเก็บข้อมูล สำหรับข้อมูลเพิ่มเติม โปรดเยี่ยมชมที่[เรียกใช้การจัดการโฟลเดอร์ผู้ช่วย](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)
    
  - **โซลูชัน:** เรียกใช้คำสั่งต่อไปนี้เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- ซึ่งอาจจะเกิดขึ้น**RetentionHold**ถูก**เปิดใช้งาน**ในกล่องจดหมาย ถ้ากล่องจดหมายที่ถูกวางไว้บน RetentionHold นโยบายการเก็บข้อมูลในกล่องจดหมายจะไม่สามารถดำเนินการในระหว่างเวลานั้น สำหรับ informaton เพิ่มเติมในการดูการตั้งค่า RetentionHold:[เก็บข้อมูลกล่องจดหมายที่เก็บ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **โซลูชัน:**
    
  - ตรวจสอบสถานะของการตั้งค่ากล่องจดหมายเฉพาะเจาะจงใน[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)RetentionHold:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - เรียกใช้คำสั่งต่อไปนี้เพื่อ**ปิดการใช้งาน**RetentionHold บนกล่องจดหมายเฉพาะ:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - ขณะนี้ เรียกใช้ใหม่ในโฟลเดอร์ที่มีการจัดการผู้ช่วย:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 เมกะไบต์ ผู้จัดการโฟลเดอร์ช่วยจะไม่ประมวลผลโดยอัตโนมัติกล่องจดหมาย
 
สำหรับข้อมูลเพิ่มเติมในนโยบายการเก็บข้อมูลในศูนย์ดูแลอัตราแลกเปลี่ยน ดู:
- [แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [เพิ่ม หรือเอาแท็กการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [วิธีการระบุชนิดของการระงับที่วางอยู่บนกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
