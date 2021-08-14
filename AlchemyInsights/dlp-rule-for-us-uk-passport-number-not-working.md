---
title: กฎ DLP ของหมายเลขหนังสือเดินทางสหรัฐอเมริกา/สหราชอาณาจักรไม่ใช้งาน
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004965"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>ปัญหากับ DLP - หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

**ปัญหา DLP กับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร**

คุณมีปัญหากับการป้องกันการสูญหายของข้อมูล **(DLP)** ไม่ใช้งานกับเนื้อหาที่มีหมายเลขหนังสือเดินทางของ **สหรัฐอเมริกา/สหราชอาณาจักร** เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.
  
ตัวอย่างเช่น นโยบายหมายเลขหนังสือเดินทาง **ของสหรัฐอเมริกา/สหราชอาณาจักร** ที่กําหนดค่าด้วยระดับความเชื่อมั่นที่ 75% ต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบเพื่อให้กฎทริกเกอร์
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** เก้าหลัก

- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลขติดกันเก้าหลัก

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่ ไม่มี Checksum

- **[นิยาม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** นโยบาย DLP มั่นใจ 75% ว่าจะถูกตรวจพบชนิดข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้เคียง 300 อักขระ:

  - ฟังก์ชันFunc_usa_uk_passportจะค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - จะพบKeyword_passportหลักจากการค้นหา

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้ทริกเกอร์นโยบายหมายเลขหนังสือเดินทาง **ของสหรัฐอเมริกา/สหราชอาณาจักร** หมายเลขหนังสือเดินทาง123456789

ดูข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่ต้องใช้ในการตรวจหาหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรเพื่อดูเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้: ชนิดข้อมูลที่ละเอียดอ่อนมีลักษณะอย่างไรกับหมายเลขหนังสือเดินทางของ [สหรัฐอเมริกา/สหราชอาณาจักร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
การใช้ชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในชนิดอื่น ให้ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับสิ่งที่ต้องใช้ในชนิดอื่นๆ ชนิดข้อมูลที่ละเอียดอ่อน [มีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  