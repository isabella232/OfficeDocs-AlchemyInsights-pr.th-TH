---
title: การเพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663532"
---
# <a name="add-external-users-to-a-distribution-group"></a>เพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย

การเพิ่มที่ติดต่อภายนอกลงในกลุ่มการแจกจ่าย (DG) เป็นกระบวนการสองขั้นตอนดังนี้
  
1. สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:
    
    1. ในศูนย์การจัดการให้ไปที่หน้าผู้ติดต่อของ**ผู้ใช้**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. เลือก**เพิ่มที่ติดต่อ**
    
    3. พิมพ์ข้อมูลสำหรับที่ติดต่อของคุณแล้วเลือก**เพิ่ม**
    
2. เพิ่มที่ติดต่อจดหมายลงใน DG ของคุณ:
    
    1. ในศูนย์การจัดการให้ไปที่หน้า**Groups**  >  [กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)กลุ่ม 
    
    2. ค้นหา DG ที่คุณต้องการเพิ่มผู้ใช้ภายนอกและเลือกกล่องโต้ตอบเพื่อเปิดกล่องโต้ตอบแก้ไข
    
    3. บนแท็บ**สมาชิก**ให้เลือก**ดูทั้งหมดและจัดการสมาชิก** 
    
    4. เลือก**เพิ่มสมาชิก**
    
    5. เลือกที่ติดต่อจดหมายที่คุณสร้างขึ้นในขั้นตอนก่อนหน้านี้แล้วเลือก**บันทึก**
    
ถ้าหลังจากทำตามขั้นตอนเหล่านี้ผู้ใช้ภายนอกของคุณไม่สามารถส่งอีเมลไปยัง DG หรือไม่ได้รับอีเมลจากอีเมลนั้นอาจเป็นไปได้ว่า DG ถูกทำเครื่องหมายให้อนุญาตอีเมลจากผู้ใช้ภายในเท่านั้น คุณสามารถตรวจสอบการกำหนดค่านี้และแก้ไขปัญหาตามคำแนะนำ[ที่นี่](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **หมายเหตุ:** คำแนะนำเหล่านี้จะไม่นำไปใช้ถ้าชนิดของกลุ่มของคุณเป็น "Microsoft ๓๖๕ group" แทนที่จะเป็น "กลุ่มการแจกจ่าย" ถ้าเป็นกรณีนี้คุณสามารถเพิ่มผู้ใช้ภายนอกลงในกลุ่มจาก Outlook ได้โดยตรง ข้อมูลรายละเอียดเกี่ยวกับ Microsoft ๓๖๕กลุ่มผู้เข้าร่วมรวมถึงคำแนะนำสำหรับการเพิ่มผู้เยี่ยมชมภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  