---
title: กฎ DLP สําหรับหมายเลขบัญชีธนาคารของสหรัฐอเมริกาไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507353"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ปัญหาเกี่ยวกับหมายเลขบัญชีธนาคารของสหรัฐฯ

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**ปัญหาเกี่ยวกับหมายเลขบัญชีธนาคารของสหรัฐฯ**

คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**เมื่อใช้ประเภทข้อมูลที่สําคัญ DLP ใน O365? ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังค้นหาเมื่อได้รับการประเมิน
  
ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐฯ**ที่กําหนดค่าด้วยระดับความเชื่อมั่นเป็น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 หลัก

- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8- 17ตัวเลขต่อเนื่องของ

- **[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มีไม่มีเช็คซัม

- **[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** นโยบาย DLP มีความมั่นใจ 75% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:

  - นิพจน์ทั่วไปRegex_usa_bank_account_numberค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคําสําคัญจากKeyword_usa_Bank_Account

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**: การตรวจสอบบัญชี 78344011

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ**การตรวจพบหมายเลขบัญชีธนาคารของสหรัฐอเมริกา**สําหรับเนื้อหาของคุณ ให้ดูในส่วนต่อไปนี้ในบทความนี้:[ประเภทข้อมูลที่สําคัญมองหาหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  