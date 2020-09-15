---
title: กฎ DLP สำหรับ SSN ไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679388"
---
# <a name="dlp-issues-with-social-security-numbers"></a>ปัญหา DLP เกี่ยวกับหมายเลขประกันสังคม

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**ปัญหา DLP เกี่ยวกับ SSNs**

คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่เป็นความลับใน Microsoft ๓๖๕ใช่หรือไม่ ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นสำหรับนโยบาย DLP ที่กำลังค้นหา 
  
ตัวอย่างเช่นสำหรับนโยบาย SSN ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๘๕% ดังต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 หลักซึ่งอาจอยู่ในรูปแบบที่จัดรูปแบบหรือรูปแบบที่ไม่มีการจัดรูปแบบ

- **[ลวดลาย:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ฟังก์ชันสี่ฟังก์ชันสำหรับ SSNs ในรูปแบบที่แตกต่างกันสี่รูปแบบดังนี้

  - Func_ssn ค้นหา SSNs ด้วยการจัดรูปแบบที่มีความแข็งแกร่งล่วงหน้า๒๐๑๑ที่จัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-ดี dddd หรือ ddd พิ่ม dddd)

  - Func_unformatted_ssn ค้นหา SSNs ด้วยการจัดรูปแบบที่มีความแข็งแกร่งล่วงหน้า๒๐๑๑ที่ได้รับการจัดรูปแบบเป็นตัวเลขติดกัน9ตัว (ddddddddd)

  - Func_randomized_formatted_ssn ค้นหา SSNs post-๒๐๑๑ที่จัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-ดี-dddd หรือ ddd dd dddd)

  - Func_randomized_unformatted_ssn ค้นหา SSNs post-๒๐๑๑ที่ได้รับการจัดรูปแบบเป็นตัวเลขที่ติดต่อกันได้9ตัว (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** ไม่มี Checksum

- **[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** นโยบาย DLP มีความมั่นใจ๘๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:

  - [ฟังก์ชัน Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคำสำคัญจาก[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ตัวอย่างของคำสำคัญประกอบด้วย: การ*รักษาความปลอดภัยทางสังคม, ความมั่นคงทางสังคม #, Soc Sec, SSN* ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP SSN: **SSN: 489-36-8350**
  
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับการตรวจพบ SSNs สำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  