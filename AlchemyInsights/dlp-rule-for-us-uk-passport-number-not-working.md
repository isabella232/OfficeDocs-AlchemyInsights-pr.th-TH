---
title: กฎ DLP สําหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977125"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>ปัญหาเกี่ยวกับ DLP -- US / UK หนังสือเดินทางหมายเลข

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ปัญหา DLP กับสหรัฐอเมริกา / สหราชอาณาจักรหมายเลขหนังสือเดินทาง**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา / UK**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365? ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหาเมื่อมีการประเมิน.
  
ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐฯ/สหราชอาณาจักร**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์
  
- **[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลข 9 หลัก

- **[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** เก้าหลักติดต่อกัน

- **[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มีไม่มีเช็คซัม

- **[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** นโยบาย DLP มี 75% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - ฟังก์ชันFunc_usa_uk_passportค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคําสําคัญจากKeyword_passport

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐอเมริกา/สหราชอาณาจักร**: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับหมายเลข Passport ของสหรัฐอเมริกา/สหราชอาณาจักรที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญค้นหาสําหรับ US/UK หมายเลขหนังสือเดินทาง](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  