---
title: กฎ DLP ของหมายเลขบัตรเครดิตไม่ใช้งาน
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005109"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>ปัญหา DLP กับหมายเลขบัตรเครดิต

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

**ปัญหา DLP กับหมายเลขบัตรเครดิต**

คุณมีปัญหากับการป้องกันการ **สูญหายของข้อมูล (DLP)** ไม่ใช้งานกับเนื้อหาที่มีหมายเลขบัตรเครดิตเมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ If so, make sure your content contains the needed information to trigger the DLP policy when it is evaluated. ตัวอย่างเช่น ถ้านโยบาย **บัตรเครดิตที่** กําหนดค่าด้วยระดับความเชื่อมั่นเป็น 85% เงื่อนไขต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบเพื่อให้กฎทริกเกอร์
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 หลักที่สามารถจัดรูปแบบหรือไม่จัดรูปแบบ (dddddddddddd) และต้องผ่านการทดสอบ Luhn

- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** รูปแบบที่ซับซ้อนและมีประสิทธิภาพมากซึ่งตรวจหาบัตรจากยี่ห้อหลักๆ ทั้งหมดทั่วโลก ได้แก่ Visa, MasterCard, Discover Card, JCB, American Express, บัตรก80บาท และบัตรช๊อบเกอร์

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** ใช่ Luhn checksum

- **[นิยาม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** นโยบาย DLP มั่นใจ 85% ว่าจะถูกตรวจพบชนิดข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้เคียง 300 อักขระ:

  - ฟังก์ชันFunc_credit_cardจะค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - ข้อใดข้อหนึ่งต่อไปนี้เป็นจริง

  - จะพบKeyword_cc_verificationจากโปรแกรม

  - พบคีย์เวิร์ดKeyword_cc_nameการค้นหา

  - ฟังก์ชันFunc_expiration_dateจะค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง

  - Checksum Pass

    ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์นโยบายหมายเลขบัตรเครดิต DLP:

  - Visa: 4485 3647 3952 7352
  
  - หมดอายุ: 2/2009

หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่ต้องใช้ในการ **ตรวจพบ** หมายเลขบัตรเครดิตในเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้ ชนิดข้อมูลที่ละเอียดอ่อนมีลักษณะอย่างไร [ต่อบัตรเครดิต#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
การใช้ชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในชนิดอื่น ให้ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับสิ่งที่ต้องใช้ในชนิดอื่นๆ ชนิดข้อมูลที่ละเอียดอ่อน [มีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  