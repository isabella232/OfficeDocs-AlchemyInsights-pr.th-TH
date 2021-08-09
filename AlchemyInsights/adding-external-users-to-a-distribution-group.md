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
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934852"
---
# <a name="add-external-users-to-a-distribution-group"></a>การเพิ่มผู้ใช้ภายนอกลงในกลุ่มการแจกจ่าย

การเพิ่มที่ติดต่อภายนอกลงในกลุ่มการแจกจ่าย (DG) เป็นกระบวนการสองขั้นตอน:
  
1. สร้างที่ติดต่อจดหมายให้กับผู้ใช้ภายนอก:
    
    1. ในศูนย์การจัดการ ให้ไปที่ **หน้า**  >  [](https://admin.microsoft.com/adminportal/home#/Contact)ที่ติดต่อของผู้ใช้ 
    
    2. เลือก **เพิ่ม** ที่ติดต่อ
    
    3. พิมพ์ข้อมูลที่ติดต่อของคุณ **แล้วเลือก** เพิ่ม
    
2. เพิ่มที่ติดต่อจดหมายไปยัง DG ของคุณ:
    
    1. ในศูนย์การจัดการ ให้ไปที่ **หน้า**  >  [กลุ่ม](https://admin.microsoft.com/adminportal/home#/groups)กลุ่ม 
    
    2. ค้นหา DG ที่คุณต้องการเพิ่มผู้ใช้ภายนอก แล้วเลือกเพื่อเปิดกล่องโต้ตอบแก้ไข
    
    3. **บนแท็บ** สมาชิก ให้เลือก **ดูทั้งหมดและจัดการ** สมาชิก 
    
    4. เลือก **เพิ่ม** สมาชิก
    
    5. เลือก ที่ติดต่อจดหมาย ที่คุณสร้างในขั้นตอนก่อนหน้า **แล้วเลือก** บันทึก
    
If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to allow only emails from internal users. คุณสามารถตรวจสอบการกําหนดค่านี้และแก้ไขได้ตามขั้นตอน[ที่นี่](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **หมายเหตุ:** คําแนะนําเหล่านี้จะไม่นําไปใช้กับถ้าชนิดกลุ่มของคุณMicrosoft 365 "กลุ่มการเผยแพร่" แทนที่จะเป็น "กลุ่มการแจกจ่าย" ถ้าเป็นกรณีนี้ คุณสามารถเพิ่มผู้ใช้ภายนอกลงในกลุ่มได้โดยตรงจากOutlook ข้อมูลรายละเอียดเกี่ยวกับMicrosoft 365ภายนอก และคําแนะนําในการเพิ่มแขกภายนอก[สามารถพบได้](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)ในบทความนี้
  