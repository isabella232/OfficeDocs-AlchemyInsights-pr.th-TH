---
title: เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814031"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect

เมื่อต้องการเปิดใช้งาน Writeback รีเซ็ตรหัสผ่านแบบบริการตนเอง ก่อนอื่น ให้เปิดใช้งานตัวเลือกการเขียนกลับใน Azure AD Connect จากเซิร์ฟเวอร์ Azure AD Connect ของคุณ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ลงชื่อเข้าใช้เซิร์ฟเวอร์ Azure AD Connect ของคุณ และเริ่มตัวช่วยสร้างการ **กําหนดค่า Azure AD Connect**
2. บนหน้า **ยินดีต้อนรับ** ให้คลิก **กําหนด** ค่า
3. บนหน้า **งานเพิ่มเติม** ให้เลือก **ปรับแต่งตัวเลือก** การซิงโครไนซ์ **แล้วคลิก** ถัดไป
4. บนหน้า **เชื่อมต่อไปยัง Azure AD** ให้ใส่ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของผู้เช่า Azure ของคุณ **แล้วคลิก** ถัดไป
5. บนหน้า **เชื่อมต่อไดเรกทอรี** และ **การกรอง Domain/OU** **ให้คลิก** ถัดไป
6. บนหน้า **ฟีเจอร์เพิ่มเติม** ให้เลือกกล่องที่อยู่ถัดจาก รหัสผ่าน **การเขียนกลับ****แล้วคลิก** ถัดไป
7. บนหน้า **พร้อมที่จะกําหนดค่า** ให้คลิก **กําหนดค่า** และรอให้กระบวนการเสร็จสิ้น
8. เมื่อคุณเห็นการกําหนดค่าเสร็จสิ้น **ให้คลิก** ออก

เมื่อเปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect ให้กําหนดค่า Azure AD SSPR เป็น writeback  เมื่อต้องการเปิดใช้งานการเขียนกลับของรหัสผ่านใน SSPR ให้เสร็จสิ้นขั้นตอนต่อไปนี้:

1. ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง
2. ค้นหาและเลือก **Azure Active Directory****คลิก รีเซ็ต** รหัสผ่าน **จากนั้นคลิก การรวมภายใน** องค์กร
3. ตั้งค่าตัวเลือกให้ **เขียนรหัสผ่านกลับลงในไดเรกทอรีภายในองค์กรของคุณใช่ไหม****เป็น** ใช่
4. ตั้งค่าตัวเลือกให้ **อนุญาตให้ผู้ใช้ปลดล็อกบัญชีโดยไม่ต้องรีเซ็ตรหัสผ่านของพวกเขา****ใช่หรือไม่ เป็น** ใช่
5. เมื่อพร้อม **ให้คลิก** บันทึก

For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  เมื่อผู้ดูแลระบบรีเซ็ตรหัสผ่านของผู้ใช้ในพอร์ทัล Azure ถ้าผู้ใช้รายนั้นติดต่อกับภายนอกหรือแฮชรหัสผ่านซิงโครไนซ์ รหัสผ่านจะถูกเขียนกลับไปยังภายในองค์กร ฟังก์ชันการฟังก์ชันนี้ต้องใช้ Azure Premium License (P1 หรือ P2) และขณะนี้ไม่ได้รับการสนับสนุนในพอร์ทัลผู้ดูแลระบบ Office
