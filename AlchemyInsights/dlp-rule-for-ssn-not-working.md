---
title: กฎ DLP สำหรับ SSN ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657378"
---
คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยตัว**เลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่เป็นความลับใน Office 365 ได้อย่างไร ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่า เนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งที่นโยบาย DLP ถูกต้อง 
  
ตัวอย่างเช่น สำหรับ SSN มีนโยบายการกำหนดค่า ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** ตัวเลข 9 หลัก ซึ่งอาจจะอยู่ในรูปแบบการจัดรูปแบบ หรือไม่จัดรูปแบบ 
    
- **[รูปแบบ:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชันที่ค้นหา SSNs ในสี่รูปแบบที่แตกต่างกัน: 
    
  - Func_ssn ค้นหา SSNs กับ 2011 ก่อนที่คาดเดายากจัดรูปแบบที่ถูกจัดรูปแบบ ด้วยเส้นประหรือช่องว่าง (ววววววววว OR ววววววววว)
    
  - Func_unformatted_ssn ค้นหา SSNs กับ 2011 ก่อนที่คาดเดายากจัดรูปแบบที่ไม่จัดรูปแบบเป็นตัวเลขติดกันเก้า (ddddddddd)
    
  - Func_randomized_formatted_ssn ค้นหา SSNs 2011 ลงรายการบัญชีที่มีการจัดรูปแบบ ด้วยเส้นประหรือช่องว่าง (ววววววววว OR ววววววววว)
    
  - Func_randomized_unformatted_ssn ค้นหา SSNs 2011 ลงรายการบัญชีที่จะไม่จัดรูปแบบเป็นตัวเลขติดกันเก้า (ddddddddd)
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** ไม่มี ไม่มี Checksum ไม่มี 
    
- **[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** นโยบาย DLP คือ 85% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ: 
    
  - [ฟังก์ชัน Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ 
    
  - พบคำสำคัญจาก[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) มีตัวอย่างของคำสำคัญ:*สังคม สังคม Soc วินาที SSN* ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP SSN: **SSN: 489-36-8350**
    
หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับ SSNs สามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหา SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

