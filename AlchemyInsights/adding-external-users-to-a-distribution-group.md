---
title: การเพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737928"
---
# <a name="add-external-users-to-a-distribution-group"></a>การเพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย

การเพิ่มผู้ติดต่อภายนอกไปยังกลุ่มการแจกจ่าย (DG) เป็นกระบวนการสองขั้นตอน:
  
1. สร้างที่ติดต่อจดหมายสำหรับผู้ใช้ภายนอก:
    
    1. ในศูนย์การจัดการให้ไปที่หน้าผู้[ติดต่อ](https://admin.microsoft.com/adminportal/home#/Contact)ของ**ผู้ใช้** >  
    
    2. เลือก**เพิ่มที่ติดต่อ**
    
    3. พิมพ์ข้อมูลสำหรับที่ติดต่อของคุณและเลือก**เพิ่ม**
    
2. เพิ่มที่ติดต่อจดหมายไปยัง DG ของคุณ:
    
    1. ในศูนย์การจัดการไป > ที่หน้า[กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)กลุ่ม**** 
    
    2. ค้นหา DG ที่คุณต้องการเพิ่มผู้ใช้ภายนอกและเลือกเพื่อเปิดกล่องโต้ตอบแก้ไข
    
    3. บนแท็บ**สมาชิก**เลือก**ดูทั้งหมดและจัดการสมาชิก** 
    
    4. เลือก**เพิ่มสมาชิก**
    
    5. เลือกที่ติดต่อจดหมายที่คุณสร้างขึ้นในขั้นตอนก่อนหน้านี้แล้วเลือก**บันทึก**
    
หากหลังจากทำตามขั้นตอนเหล่านี้ผู้ใช้ภายนอกของคุณไม่สามารถส่งเมลไปยัง DG หรือไม่ได้รับเมลจากมันอาจเป็นไปได้ว่า DG ถูกทำเครื่องหมายให้อนุญาตเฉพาะผู้ใช้ภายในเท่านั้น คุณสามารถตรวจสอบการกำหนดค่านี้และแก้ไขได้ตามคำแนะนำที่[นี่](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **หมายเหตุ:** คำแนะนำเหล่านี้ไม่ได้นำไปใช้ถ้าชนิดของกลุ่มของคุณคือ "Office ๓๖๕กลุ่ม" แทน "กลุ่มการแจกจ่าย" ถ้าเป็นกรณีนี้คุณสามารถเพิ่มผู้ใช้ภายนอกลงในกลุ่มจาก Outlook ได้โดยตรง ข้อมูลรายละเอียดเกี่ยวกับ Office ๓๖๕กลุ่มผู้เข้าพักและคำแนะนำสำหรับการเพิ่มผู้เข้าพักภายนอกสามารถพบได้ใน[บทความนี้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  