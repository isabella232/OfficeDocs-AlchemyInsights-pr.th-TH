---
title: กฎ DLP สำหรับเราหมายเลขบัญชีธนาคารไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529902"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>การตัดสินค้าจากคลัง DLP กับเราหมายเลขบัญชีธนาคาร

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
  