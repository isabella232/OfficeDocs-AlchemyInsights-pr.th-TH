---
title: กฎ DLP สําหรับสหรัฐอเมริกา / สหราชอาณาจักรหนังสือเดินทางหมายเลขไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507317"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>ปัญหาเกี่ยวกับ DLP -- หมายเลขหนังสือเดินทางสหรัฐ / สหราชอาณาจักร

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ปัญหาเกี่ยวกับหมายเลขหนังสือเดินทางของสหรัฐฯ/สหราชอาณาจักร**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขหนังสือเดินทางสหรัฐ / สหราชอาณาจักร**เมื่อใช้ประเภทข้อมูลที่สําคัญ DLP ใน O365? ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังค้นหาเมื่อได้รับการประเมิน
  
ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** เก้าหลัก

- **[รูปแบบ: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลข 9 ตัวติดต่อกัน

- **[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มีไม่มีเช็คซัม

- **[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** นโยบาย DLP มีความมั่นใจ 75% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - ฟังก์ชันFunc_usa_uk_passportค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคําสําคัญจากKeyword_passport

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร**: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับการตรวจพบหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรสําหรับเนื้อหาของคุณ ให้ดูในส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ชนิดข้อมูลที่ละเอียดอ่อนมองหาหมายเลขหนังสือเดินทางสหรัฐอเมริกา /สหราชอาณาจักร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  