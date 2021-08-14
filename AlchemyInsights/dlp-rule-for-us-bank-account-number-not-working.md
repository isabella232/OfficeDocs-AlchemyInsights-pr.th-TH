---
title: กฎ DLP ของหมายเลขบัญชีธนาคารของสหรัฐอเมริกาไม่ใช้งาน
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005037"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

**ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา**

คุณมีปัญหากับการป้องกันการ **สูญหายของข้อมูล (DLP)** ไม่ใช้งานกับเนื้อหาที่มีหมายเลขบัญชีธนาคารของ **สหรัฐอเมริกา** เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.
  
ตัวอย่างเช่น ในนโยบายหมายเลขบัญชีธนาคาร **ของสหรัฐอเมริกา** ที่กําหนดค่าด้วยระดับความเชื่อมั่นที่ 85% นโยบายต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบเพื่อให้กฎทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 หลัก

- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลขติดกัน 8-17 หลัก

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่ ไม่มี Checksum

- **[นิยาม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** นโยบาย DLP มั่นใจ 75% ว่าจะถูกตรวจพบชนิดข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้เคียง 300 อักขระ:

  - นิพจน์ทั่วไปRegex_usa_bank_account_numberค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - จะพบKeyword_usa_Bank_Accountจากโปรแกรม

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์นโยบาย **หมายเลขบัญชีธนาคาร** ของสหรัฐอเมริกา: การตรวจสอบหมายเลข78344011

For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: What the Sensitive Information Types look for US Bank Account [Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
การใช้ชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในชนิดอื่น ให้ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับสิ่งที่ต้องใช้ในชนิดอื่นๆ ชนิดข้อมูลที่ละเอียดอ่อน [มีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  