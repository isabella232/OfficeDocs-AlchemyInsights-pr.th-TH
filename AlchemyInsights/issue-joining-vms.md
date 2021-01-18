---
title: ปัญหาในการเข้าร่วม VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885659"
---
# <a name="issue-joining-vms"></a>ปัญหาในการเข้าร่วม VMs

เมื่อต้องการแก้ไขปัญหาที่เกิดขึ้นขณะพยายามเข้าร่วม VMs ให้ดำเนินการตามขั้นตอนต่อไปนี้:

1. ลองลงชื่อเข้าใช้โดยใช้รูปแบบ **UPN** (ตัวอย่างเช่น ' joeuser@contoso.com ') แทนที่จะเป็นรูปแบบ **SAMAccountName** (' CONTOSO\joeuser ')
2. ตรวจสอบให้แน่ใจว่าคุณได้เปิดใช้งานการซิงโครไนซ์รหัสผ่านให้สอดคล้องกับขั้นตอนที่ระบุไว้ในคู่มือ *การเริ่มต้น* ใช้งาน
3. ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ได้รับผลกระทบไม่ใช่บัญชีภายนอกในผู้เช่า Azure AD ผู้ใช้ภายนอกไม่สามารถลงชื่อเข้าใช้โดเมนที่มีการจัดการได้เนื่องจากบริการ Domain AD Azure ไม่มีข้อมูลประจำตัวสำหรับบัญชีผู้ใช้ดังกล่าว
4. ถ้าบัญชีผู้ใช้ที่ได้รับผลกระทบเป็นบัญชีผู้ใช้ cloud เท่านั้นให้ตรวจสอบให้แน่ใจว่าผู้ใช้ได้เปลี่ยนรหัสผ่านของพวกเขาหลังจากที่คุณเปิดใช้งาน Azure AD Domain Services แล้ว ขั้นตอนนี้ทำให้เกิด hashes ข้อมูลประจำตัวที่จำเป็นสำหรับบริการโดเมน AD Azure ที่จะถูกสร้างขึ้น
5. ถ้ามีการซิงโครไนซ์บัญชีผู้ใช้ที่ได้รับผลกระทบจากไดเรกทอรีภายในองค์กรให้ตรวจสอบว่ามีการกำหนดค่าการเผยแพร่ AD Azure ที่แนะนำให้ทำการซิงโครไนซ์ทั้งหมดหรือไม่
6. ถ้าปัญหายังคงมีอยู่หลังจากยืนยันขั้นตอนที่4ให้ดำเนินการคำสั่งต่อไปนี้จากเครื่องซิงค์ของคุณ:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.