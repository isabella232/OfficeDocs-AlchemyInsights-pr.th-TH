---
title: กฎ DLP สำหรับเราหมายเลขบัญชีธนาคารไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657018"
---
คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยหมาย**เลขบัญชีธนาคารของสหรัฐอเมริกา**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่าเนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งนโยบาย DLP จะค้นหาเมื่อถูกประเมิน 
  
ตัวอย่างเช่น**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**โยบายการกำหนดค่า ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์: 
  
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลข 8-17 
    
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 ตัวเลขที่ต่อเนื่องกัน 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มี ไม่มี Checksum ไม่มี 
    
- **[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** นโยบาย DLP คือ 75% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ: 
    
  - นิพจน์ทั่วไป Regex_usa_bank_account_number ค้นหาเนื้อหาที่ตรงกับรูปแบบ
    
  - พบคำสำคัญจาก Keyword_usa_Bank_Account
    
    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**นโยบาย: 78344011 บัญชีกระแสรายวัน 
    
สำหรับข้อมูลเพิ่มเติมบนสิ่งจำเป็นสำหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**เพื่อพบกับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหาหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

