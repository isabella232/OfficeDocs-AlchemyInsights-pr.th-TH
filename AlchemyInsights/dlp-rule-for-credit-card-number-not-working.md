---
title: กฎ DLP สําหรับหมายเลขบัตรเครดิตไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932462"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>ปัญหา DLP กับหมายเลขบัตรเครดิต

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**ปัญหา DLP กับหมายเลขบัตรเครดิต**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัตรเครดิต**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365? ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นเพื่อทริกเกอร์นโยบาย DLP เมื่อมีประเมิน ตัวอย่างเช่น สําหรับ**นโยบายบัตรเครดิต**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% มีการประเมินต่อไปนี้ และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 หลักซึ่งสามารถจัดรูปแบบหรือไม่ได้จัดรูปแบบ (dddddddddddddddddddddd) และจะต้องผ่านการทดสอบ Luhn

- **[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** รูปแบบที่ซับซ้อนและแข็งแกร่งมากที่ตรวจจับการ์ดจากแบรนด์สําคัญๆ ทั่วโลก รวมถึง Visa, MasterCard, Discover Card, JCB, American Express, บัตรของขวัญ และบัตรอาหาร

- **[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** ใช่, การตรวจสอบ Luhn

- **[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - ฟังก์ชันFunc_credit_cardค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - หนึ่งต่อไปนี้เป็นจริง:

  - พบคําสําคัญจากKeyword_cc_verification

  - พบคําหลักจากKeyword_cc_name

  - ฟังก์ชันFunc_expiration_dateค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง

  - เช็คซัมผ่าน

    ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบายหมายเลขบัตรเครดิต DLP:

  - วีซ่า: 4485 3647 3952 7352
  
  - หมดอายุ: 2/2009

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งจําเป็นสําหรับ**หมายเลขบัตรเครดิต**ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ชนิดข้อมูลที่สําคัญที่มองหาบัตรเครดิต #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  