---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317150"
---
มีปัญหาในการเก็บถาวรรายการไปยังกล่องจดหมายการเก็บถาวร ตรวจสอบให้แน่ใจว่า คุณได้ดำเนินการขั้นตอนต่อไปนี้:
  
1. ยืนยันว่า การ**เก็บถาวรกล่องจดหมาย**ได้ถูกเปิดใช้งาน ถ้า ไม่มี ทำตามขั้นตอนใน[บทความนี้](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานการเก็บถาวรกล่องจดหมาย 
    
2. ในศูนย์ดูแล Exchange เลือก**แท็กการเก็บข้อมูล**ที่อยู่ภายใต้การ**บริหารการปฏิบัติตามกฎระเบียบ**สร้าง**แท็กการเก็บข้อมูล**ที่ มีการดำเนินการ**ย้ายไปยังที่เก็บถาวร**ที่ประกอบด้วย**อายุการเก็บข้อมูล**ที่ต้องการ
    
3. ในศูนย์ดูแล Exchange เลือก**นโยบายการเก็บข้อมูล**สร้าง**นโยบายการเก็บข้อมูล**และเพิ่มแท็กเก็บข้อมูลของคุณ**ย้ายไปยังที่เก็บถาวร**ที่นโยบาย 
    
4. [กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)กับกล่องจดหมายของผู้ใช้ที่ระบุ จะใช้นโยบายเดียวกันกับ**หลัก**และกล่องจดหมาย**เก็บถาวร** 
    
กล่องจดหมายของผู้ใช้ควรมีมีนโยบายการเก็บถาวรเพื่อย้ายรายการไปยังกล่องจดหมายการเก็บถาวรในขณะนี้ คุณอาจจำเป็นในการบังคับใช้การจัดการโฟลเดอร์ผู้ช่วย (MFA) เมื่อต้องการเรียกใช้ และใช้การตั้งค่าใหม่กับกล่องจดหมายของผู้ใช้ เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

ต้องการข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ดูการ[ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  

