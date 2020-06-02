---
title: กฎ DLP สําหรับหมายเลขบัตรเครดิตไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507425"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>ปัญหาเกี่ยวกับหมายเลขบัตรเครดิต DLP

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ปัญหาเกี่ยวกับหมายเลขบัตรเครดิต DLP**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัตรเครดิต**เมื่อใช้ประเภทข้อมูลที่สําคัญ DLP ใน O365? ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นในการเรียกใช้นโยบาย DLP เมื่อได้รับการประเมิน ตัวอย่างเช่น สําหรับ**นโยบายบัตรเครดิต**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 หลักที่สามารถจัดรูปแบบหรือไม่ได้จัดรูปแบบ (ddddddddddddd) และต้องผ่านการทดสอบ Luhn

- **[รูปแบบ: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** รูปแบบที่ซับซ้อนมากและแข็งแกร่งที่ตรวจพบบัตรจากแบรนด์สําคัญทั้งหมดทั่วโลกรวมทั้งวีซ่ามาสเตอร์การ์ดการ์ดค้นพบ JCB อเมริกันเอ็กซ์เพรสบัตรของขวัญและบัตรร้านอาหาร

- **[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** ใช่ เช็คซัมลูน

- **[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** นโยบาย DLP มีความมั่นใจ 85% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - ฟังก์ชันFunc_credit_cardค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - หนึ่งในต่อไปนี้เป็นจริง:

  - พบคําสําคัญจากKeyword_cc_verification

  - พบคําสําคัญจาก Keyword_cc_name

  - ฟังก์ชันFunc_expiration_dateค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง

  - เช็คซัมผ่าน

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบายหมายเลขบัตรเครดิต DLP:

  - วีซ่า: 4485 3647 3952 7352
  
  - หมดอายุ: 2/2009

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ**การตรวจพบหมายเลขบัตรเครดิต**สําหรับเนื้อหาของคุณ โปรดดูส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ประเภทข้อมูลที่สําคัญมองหาบัตรเครดิต#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  