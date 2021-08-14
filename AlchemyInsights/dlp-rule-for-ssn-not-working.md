---
title: กฎ DLP ของ SSN ไม่ใช้งาน
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005001"
---
# <a name="dlp-issues-with-social-security-numbers"></a>ปัญหา DLP กับหมายเลขประกันสังคม

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

**ปัญหา DLP กับ SSN**

คุณมีปัญหากับการป้องกันการสูญหายของข้อมูล **(DLP)** ไม่สามารถใช้งานกับเนื้อหาที่มีหมายเลขประกันสังคม **(SSN)** เมื่อใช้ชนิดข้อมูลที่เป็นความลับในMicrosoft 365หรือไม่ If so, make sure your content contains the needed information for what the DLP policy is looking. 
  
ตัวอย่างเช่น เมื่อกําหนดค่านโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% นโยบายต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบเพื่อให้กฎทริกเกอร์
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 หลักซึ่งอาจอยู่ในรูปแบบที่มีการจัดรูปแบบหรือไม่จัดรูปแบบ

- **[รูปแบบ:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชันจะค้นหา SSN ในรูปแบบที่แตกต่างกันสี่รูปแบบ:

  - Func_ssn SSN ที่มีการจัดรูปแบบ strong ก่อนปี 2554 ที่ถูกจัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-dd-dddd OR ddd dddd)

  - Func_unformatted_ssn SSN ที่มีการจัดรูปแบบอย่างรัดกุมก่อนปี 2554 ที่ไม่มีการจัดรูปแบบเป็นตัวเลข 9 หลักติดกัน (dddddddd)

  - Func_randomized_formatted_ssnจะค้นหา SSN หลัง 2011 ที่ถูกจัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-dddd หรือ ddd dddd OR ddddd)

  - Func_randomized_unformatted_ssn SSN หลัง 2011 ที่ไม่มีการจัดรูปแบบเป็นตัวเลขติดกันเก้าหลัก (dddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** ไม่ ไม่มี Checksum

- **[นิยาม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** นโยบาย DLP มั่นใจ 85% ว่าจะถูกตรวจพบชนิดข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้เคียง 300 อักขระ:

  - ฟังก์ชัน [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) จะค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - จะพบ [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) หลักจากการค้นหา ตัวอย่างของคําหลักประกอบด้วย: *Social Security, Social Security#, Soc Sec , SSN* ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์นโยบาย DLP SSN: **SSN: 489-36-8350**
  
For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
การใช้ชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในชนิดอื่น ให้ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับสิ่งที่ต้องใช้ในชนิดอื่นๆ ชนิดข้อมูลที่ละเอียดอ่อน [มีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  