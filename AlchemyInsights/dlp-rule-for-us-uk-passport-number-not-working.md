---
title: กฎ DLP สำหรับสหรัฐอเมริกา / หมาย เลขหนังสือเดินทางสหราชอาณาจักรที่ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404400"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>ปัญหาเกี่ยวกับ DLP - สหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร

คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่าเนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งนโยบาย DLP จะค้นหาเมื่อถูกประเมิน 
  
ตัวอย่างเช่น สำหรับการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**นโยบายการตั้งค่าคอนฟิก ด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์ 
  
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลขเก้าหลัก 
    
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** ตัวเลขที่ต่อเนื่องกันเก้า 
    
- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มี ไม่มี Checksum ไม่มี 
    
- **[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** นโยบาย DLP คือ 75% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ: 
    
  - ฟังก์ชัน Func_usa_uk_passport ค้นหาเนื้อหาที่ตรงกับรูปแบบ
    
  - พบคำสำคัญจาก Keyword_passport
    
    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**นโยบาย: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789 
    
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับประเทศ / หมายเลขหนังสือเดินทางสหราชอาณาจักรสามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ดูหัวข้อต่อไปนี้ในบทความนี้:[มองหาสิ่งเป็นความลับชนิดข้อมูลสำหรับสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

