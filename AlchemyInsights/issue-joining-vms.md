---
title: ปัญหาในการเข้าร่วม IM
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
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088091"
---
# <a name="issue-joining-vms"></a>ปัญหาในการเข้าร่วม IM

เมื่อต้องการแก้ไขปัญหาที่เกิดขึ้นขณะพยายามเข้าร่วม IM ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. พยายามลงชื่อเข้าใช้โดยใช้รูปแบบ **UPN** (ตัวอย่างเช่น 'joeuser@contoso.com') แทนรูปแบบ **SAMAccountName** ('CONTOSO\joeuser')
2. ตรวจสอบให้แน่ใจว่าคุณได้เปิดใช้งานการซิงโครไนซ์รหัสผ่านตามขั้นตอนที่อธิบายไว้ *ในคู่มือ* การเริ่มต้นใช้งาน
3. ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ได้รับผลกระทบไม่ใช่บัญชีภายนอกในผู้เช่า Azure AD ผู้ใช้ภายนอกไม่สามารถลงชื่อเข้าใช้โดเมนที่มีการจัดการได้ เนื่องจาก Azure AD Domain Services ไม่มีข้อมูลรับรองของบัญชีผู้ใช้ดังกล่าว
4. ถ้าบัญชีผู้ใช้ที่ได้รับผลกระทบเป็นบัญชีผู้ใช้ระบบคลาวด์เท่านั้น ตรวจสอบให้แน่ใจว่าผู้ใช้เปลี่ยนรหัสผ่านหลังจากที่คุณเปิดใช้งาน Azure AD Domain Services แล้ว ขั้นตอนนี้จะเป็นสาเหตุให้ระบบสร้างข้อมูลรับรองความถูกต้องของ Azure AD Domain Services
5. ถ้าบัญชีผู้ใช้ที่ได้รับผลกระทบได้รับการซิงโครไนซ์จากไดเรกทอรีภายในองค์กร ให้ตรวจสอบว่า Azure AD เชื่อมต่อ ที่แนะเชื่อมต่อได้รับการกําหนดค่าให้ซิงโครไนซ์ทั้งหมด
6. ถ้าปัญหายังคงอยู่หลังจากยืนยันขั้นตอนที่ 4 ให้เรียกใช้สั่งต่อไปนี้จากเครื่องซิงค์ของคุณ:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.