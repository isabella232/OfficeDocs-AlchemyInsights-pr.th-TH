---
title: เปิดใช้งาน Writeback รหัสผ่านใน Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093374"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>เปิดใช้งาน Writeback รหัสผ่านใน Azure AD Connect

เมื่อต้องการเปิดใช้งาน Writeback รีเซ็ตรหัสผ่านแบบบริการตนเอง ก่อนอื่น ให้เปิดใช้งานตัวเลือก Writeback ใน Azure AD Connect จากเซิร์ฟเวอร์ Azure AD Connect ของคุณ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ลงชื่อเข้าใช้เซิร์ฟเวอร์ Azure AD Connect ของคุณและเริ่มตัวช่วยสร้างการ **กําหนดค่า Azure AD Connect**
2. บนหน้า **ยินดีต้อนรับ** ให้คลิก **กําหนด** ค่า
3. บนหน้า **งานเพิ่มเติม** ให้เลือกตัวเลือก **ปรับแต่งการ** ซิงโครไนซ์ **แล้วคลิก** ถัดไป
4. บนหน้า **เชื่อมต่อไปยัง Azure AD ให้** ใส่ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของผู้เช่า Azure ของคุณ **แล้วคลิก** ถัดไป
5. บนหน้า **การกรอง เชื่อมต่อ** ไดเรกทอรี **และโดเมน/OU** **ให้คลิก** ถัดไป
6. บนหน้า **ฟีเจอร์เพิ่มเติม** ให้เลือกกล่องที่อยู่ถัดจาก Password **Writeback****แล้วคลิก** ถัดไป
7. บนหน้า **พร้อมที่จะกําหนดค่า** ให้คลิก **กําหนด** ค่า และรอให้กระบวนการเสร็จสิ้น
8. เมื่อคุณเห็นการกําหนดค่าเสร็จสิ้น **ให้คลิก** ออก

เมื่อเปิดใช้งาน Writeback ของรหัสผ่านใน Azure AD Connect ให้กําหนดค่า Azure AD SSPR for writeback  เมื่อต้องการเปิดใช้งาน Writeback ของรหัสผ่านใน SSPR ให้เสร็จสิ้นขั้นตอนต่อไปนี้:

1. ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง
2. ค้นหาและเลือก **Azure Active Directory****คลิกรีเซ็ต** รหัสผ่าน จากนั้นคลิก **การรวมภายใน** องค์กร
3. ตั้งค่าตัวเลือกให้ **เขียนรหัสผ่านกลับลงในไดเรกทอรีภายในองค์กรของคุณใช่ไหม****เป็น** ใช่
4. ตั้งค่าตัวเลือกให้ **อนุญาตให้ผู้ใช้ปลดล็อกบัญชีโดยไม่ต้องรีเซ็ตรหัสผ่านของพวกเขาหรือไม่****เป็น** ใช่
5. เมื่อพร้อม **ให้คลิก** บันทึก

For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  เมื่อผู้ดูแลระบบรีเซ็ตรหัสผ่านของผู้ใช้ในพอร์ทัล Azure ถ้าผู้ใช้นั้นติดต่อกับภายนอกหรือแฮชรหัสผ่านซิงโครไนซ์ รหัสผ่านจะถูกเขียนกลับไปยังภายในองค์กร หน้าที่การใช้งานนี้ต้องใช้ Azure Premium License (P1 หรือ P2) และในขณะนี้ไม่ได้รับการสนับสนุนในพอร์ทัลผู้ดูแลระบบ Office
