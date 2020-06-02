---
title: กฎ DLP สําหรับ SSN ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507389"
---
# <a name="dlp-issues-with-social-security-numbers"></a>ปัญหาเกี่ยวกับหมายเลข DLP ประกันสังคม

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ปัญหาเกี่ยวกับ SSNs DLP**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่สําคัญใน Microsoft 365 หรือไม่ หากเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับนโยบาย DLP กําลังค้นหา 
  
ตัวอย่างเช่น สําหรับนโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎเพื่อทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 หลักซึ่งอาจอยู่ในรูปแบบการจัดรูปแบบหรือไม่จัดรูปแบบ

- **[รูปแบบ: 10000](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชั่นมองหา SSNs ในรูปแบบที่แตกต่างกันสี่:

  - Func_ssnพบ SSNs ที่มีการจัดรูปแบบที่แข็งแกร่งก่อนปี 2011 ซึ่งจัดรูปแบบด้วยเครื่องหมายขีดกลางหรือช่องว่าง (ddd-ddd-ddd หรือ ddd ddd)

  - Func_unformatted_ssnพบ SSNs ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ที่ไม่มีการจัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (ddddddddd)

  - Func_randomized_formatted_ssnค้นหา SSNs post-2011 ที่มีการจัดรูปแบบด้วยเครื่องหมายขีดกลางหรือช่องว่าง (ddd-ddd-ddd หรือ ddd ddd)

  - Func_randomized_unformatted_ssnพบ SSNs โพสต์-2011 ที่ไม่ถูกจัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (ddddddddd)

- **[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** ไม่มีไม่มีเช็คซัม

- **[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** นโยบาย DLP มีความมั่นใจ 85% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - [ฟังก์ชันFunc_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคําสําคัญจาก[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) ตัวอย่างของคําหลักรวมถึง:*ประกันสังคม, ประกันสังคม # # , Soc Sec , SSN* . ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย DLP SSN: **SSN: 489-36-8350**
  
สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ SSNs ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูในส่วนต่อไปนี้ในบทความนี้:[ชนิดข้อมูลละเอียดอ่อนค้นหา SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  