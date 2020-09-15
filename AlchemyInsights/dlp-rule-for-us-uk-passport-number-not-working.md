---
title: กฎ DLP สำหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรไม่ทำงาน
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679243"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>ปัญหาเกี่ยวกับ DLP-หมายเลขพาสปอร์ตของสหรัฐอเมริกา/UK

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**ปัญหา DLP กับเลขพาสปอร์ตของสหรัฐอเมริกา/UK**

คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร** เมื่อใช้ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ใน O365 ใช่หรือไม่ ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นสำหรับสิ่งที่นโยบาย DLP กำลังค้นหาเมื่อมีการประเมิน
  
ตัวอย่างเช่นสำหรับนโยบาย **หมายเลขหนังสือเดินทางสหรัฐอเมริกา/UK** ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๗๕% ต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** เก้าหลัก

- **[ลวดลาย:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลขที่ติดต่อกันได้9ตัว

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มี Checksum

- **[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** นโยบาย DLP มีความมั่นใจ๗๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:

  - ฟังก์ชัน Func_usa_uk_passport ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคำสำคัญจาก Keyword_passport

    ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย **หมายเลขหนังสือเดินทางสหรัฐอเมริกา/UK** : หมายเลขหนังสือเดินทางของสหรัฐอเมริกา๑๒๓๔๕๖๗๘๙

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/UK ที่จะถูกตรวจพบสำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับของหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  