---
title: นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ไม่ทำงาน
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740529"
---
# <a name="retention-policies-in-exchange-admin-center"></a>นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange

ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหาเกี่ยวกับนโยบายการเก็บข้อมูล

 **ปัญหา:** นโยบายการเก็บข้อมูลที่สร้างขึ้นใหม่หรือที่อัปเดตในศูนย์การจัดการ Exchange จะไม่ถูกนำไปใช้กับกล่องจดหมายหรือรายการจะไม่ถูกย้ายไปยังกล่องจดหมายเก็บถาวรหรือถูกลบ 
  
 **สาเหตุราก:**
  
- ซึ่งอาจเป็นเพราะ **ผู้ช่วยโฟลเดอร์** ที่มีการจัดการยังไม่ได้ประมวลผลกล่องจดหมายของผู้ใช้ ผู้ช่วยโฟลเดอร์ที่ได้รับการจัดการพยายามดำเนินการทุกกล่องจดหมายในองค์กร cloud-based ของคุณทุกๆ7วัน ถ้าคุณเปลี่ยนแท็กการเก็บข้อมูลหรือนำนโยบายการเก็บข้อมูลอื่นไปใช้กับกล่องจดหมายคุณสามารถรอจนกว่าโฟลเดอร์ที่ได้รับการจัดการช่วยประมวลผลกล่องจดหมายหรือคุณสามารถเรียกใช้ cmdlet เริ่มต้น ManagedFolderAssistant เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการเพื่อประมวลผลกล่องจดหมายที่เฉพาะเจาะจงได้ การเรียกใช้ cmdlet นี้มีประโยชน์สำหรับการทดสอบหรือการแก้ไขปัญหานโยบายการเก็บข้อมูลหรือการตั้งค่าแท็กการเก็บข้อมูล สำหรับข้อมูลเพิ่มเติมให้เยี่ยมชม[เรียกใช้ตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการ](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)
    
  - **วิธีแก้ไข:** เรียกใช้คำสั่งต่อไปนี้เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่เฉพาะเจาะจง:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- สิ่งนี้อาจเกิดขึ้นถ้า **RetentionHold** ถูก **เปิดใช้งาน** ในกล่องจดหมาย ถ้ามีการวางกล่องจดหมายบน RetentionHold นโยบายการเก็บข้อมูลในกล่องจดหมายจะไม่ถูกประมวลผลในระหว่างช่วงเวลานั้น สำหรับสนใจเพิ่มเติมเกี่ยวกับการตั้งค่า RetentionHold ให้ดูที่การ[ระงับการเก็บข้อมูลในกล่องจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **วิธีแก้ไข**
    
  - ตรวจสอบสถานะของการตั้งค่า RetentionHold บนกล่องจดหมายที่เฉพาะเจาะจงใน [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - เรียกใช้คำสั่งต่อไปนี้เพื่อ **ปิดใช้งาน** RetentionHold ในกล่องจดหมายที่เฉพาะเจาะจง:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - ในตอนนี้ให้เรียกใช้ตัวช่วยสร้างโฟลเดอร์ที่ได้รับการจัดการอีกครั้ง:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า10เมกะไบต์ผู้ช่วยโฟลเดอร์ที่มีการจัดการจะไม่ประมวลผลกล่องจดหมายโดยอัตโนมัติ
 
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ให้ดูที่:
- [แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [นำนโยบายการเก็บข้อมูลไปใช้กับกล่องจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [การเพิ่มหรือเอาแท็กการเก็บข้อมูลออก](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [วิธีระบุชนิดของการเก็บไว้ในกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
