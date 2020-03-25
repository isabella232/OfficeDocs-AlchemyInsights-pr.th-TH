---
title: กฎ DLP สําหรับ SSN ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932555"
---
# <a name="dlp-issues-with-social-security-numbers"></a>ปัญหา DLP กับหมายเลขประกันสังคม

**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล

ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล) คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้ อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ

**ปัญหา DLP กับ SSNs**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่สําคัญใน Office 365 หรือไม่ ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหา. 
  
ตัวอย่างเช่น สําหรับนโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 หลัก ซึ่งอาจจะเป็นรูปแบบที่จัดรูปแบบหรือรูปแบบไม่ได้จัดรูปแบบ

- **[รูปแบบ: รูปแบบ](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชั่นมองหา SSNs ในสี่รูปแบบที่แตกต่างกัน:

  - Func_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ที่มีการจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd dddd)

  - Func_unformatted_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ซึ่งยังไม่ได้จัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (dddddddddd)

  - Func_randomized_formatted_ssnพบ SSN หลัง 2011 ที่ถูกจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd ddd dddd)

  - Func_randomized_unformatted_ssnพบ SSN หลัง 2011 ที่ยังไม่ฟอร์แมตเป็นตัวเลขติดต่อกันเก้าหลัก (ddddddddddd)

- **[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** ไม่มีไม่มีเช็คซัม

- **[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - [ฟังก์ชันFunc_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคําสําคัญจาก[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ตัวอย่างของคําสําคัญได้แก่:*ประกันสังคม, ประกันสังคม# Soc Sec, SSN* ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย DLP SSN: **SSN: 489-36-8350**
  
สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ SSNs จะถูกตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญที่มองหา SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  