---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762384"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายอีเมลไปยังกล่องจดหมายการเก็บถาวร
 
1. ยืนยันว่า การ**เก็บถาวรกล่องจดหมาย**ได้ถูกเปิดใช้งาน ถ้า ไม่มี ใช้ขั้นตอนต่าง ๆ ใน[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานการเก็บถาวรกล่องจดหมาย

2. จัดเก็บข้อความโดยอัตโนมัติไปยังกล่องจดหมายการเก็บถาวร แท็กเก็บข้อมูลที่ มีการดำเนินการ**ย้ายที่เก็บถาวร**ต้องถูกตั้งค่าเพื่อ**นำไปใช้กับแท็กกล่องจดหมายทั้งหมด (ค่าเริ่มต้น) โดยอัตโนมัติ** ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กที่เก็บถาวรเริ่มต้น](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)
    
3. ถัดไป เพิ่มแท็ก**เก็บถาวร**นโยบายการเก็บข้อมูลของคุณ เลือก**นโยบายการเก็บข้อมูล**ในศูนย์ดูแล Exchange, > เพิ่มการ**ย้ายไปยังการเก็บถาวรแท็ก**> นโยบายการ**บันทึก** 
    
4. ขณะนี้[กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)กับกล่องจดหมายของผู้ใช้ที่เฉพาะเจาะจง จะใช้นโยบายเดียวกันกับ**หลัก**และกล่องจดหมาย**เก็บถาวร** 
    
คุณอาจจำเป็นในการบังคับใช้การจัดการโฟลเดอร์ผู้ช่วย (MFA) เมื่อต้องการเรียกใช้ และใช้การตั้งค่าใหม่กับกล่องจดหมายของผู้ใช้ เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ดู[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  

