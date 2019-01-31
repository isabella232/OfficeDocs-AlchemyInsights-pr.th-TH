---
title: กฎ DLP สำหรับหมายเลขบัตรเครดิตที่ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657486"
---
คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยหมาย**เลขบัตรเครดิต**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ ถ้าเป็นเช่นนั้น ให้แน่ใจว่า เนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นเพื่อทริกเกอร์นโยบาย DLP เมื่อถูกประเมิน ตัวอย่างเช่น สำหรับ**บัตรเครดิตนโยบาย**การตั้งค่าคอนฟิก ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์: 
  
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 หลักซึ่งการจัดรูปแบบหรือไม่จัดรูปแบบ (dddddddddddddddd) และต้องผ่านการทดสอบ Luhn 
    
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** รูปแบบที่สมบูรณ์ และซับซ้อนมากที่ตรวจพบการ์ดจากทั้งหมดหลักยี่ห้อทั่วโลก รวมทั้งวีซ่า Mastercard ค้นหาบัตร JCB อเมริกันเอ็กซ์เพรส บัตรของขวัญ และบัตร diner 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** ใช่ ตัวนับไว้ Luhn 
    
- **[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** นโยบาย DLP คือ 85% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ: 
    
  - ฟังก์ชัน Func_credit_card ค้นหาเนื้อหาที่ตรงกับรูปแบบ
    
  - ต่อไปนี้เป็นจริง: 
    
  - พบคำสำคัญจาก Keyword_cc_verification
    
  - พบคำสำคัญจาก Keyword_cc_name
    
  - ฟังก์ชัน Func_expiration_date ค้นหาวันที่ในรูปแบบวันที่ถูกต้อง
    
  - Checksum ผ่านไป
    
    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP หมายเลขบัตรเครดิต:
    
  - วีซ่า: การ 7352 3952 3647 4485 
    
  - หมดอายุ: 2/2009
    
สำหรับข้อมูลเพิ่มเติมบนสิ่งจำเป็นสำหรับ**หมายเลขบัตรเครดิต**สามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหาบัตรเครดิต #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

