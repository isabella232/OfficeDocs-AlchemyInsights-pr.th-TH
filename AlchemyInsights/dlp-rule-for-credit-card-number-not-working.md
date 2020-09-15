---
title: กฎ DLP สำหรับหมายเลขบัตรเครดิตไม่ทำงาน
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679460"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>ปัญหา DLP ที่มีหมายเลขบัตรเครดิต

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**ปัญหา DLP ที่มีหมายเลขบัตรเครดิต**

คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขบัตรเครดิต** เมื่อใช้ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ใน O365 ใช่หรือไม่ ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นในการทริกเกอร์นโยบาย DLP เมื่อถูกประเมิน ตัวอย่างเช่นสำหรับ **นโยบายบัตรเครดิต** ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๘๕% รายการต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** ตัวเลข16หลักที่สามารถจัดรูปแบบหรือจัดรูปแบบ (dddddddddddddddd) และต้องผ่านการทดสอบ Luhn

- **[ลวดลาย:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** รูปแบบที่มีความซับซ้อนและมีประสิทธิภาพมากที่ตรวจจับบัตรจากแบรนด์หลักๆทั้งหมดทั่วโลกรวมถึงวีซ่ามาสเตอร์การ์ดค้นพบบัตรซีเจซี, American Express, บัตรของขวัญและบัตร diner

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** ใช่ Luhn checksum

- **[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** นโยบาย DLP มีความมั่นใจ๘๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:

  - ฟังก์ชัน Func_credit_card ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - อย่างใดอย่างหนึ่งต่อไปนี้เป็นจริง:

  - พบคำสำคัญจาก Keyword_cc_verification

  - พบคำสำคัญจาก Keyword_cc_name

  - ฟังก์ชัน Func_expiration_date ค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง

  - Checksum ที่ผ่านการตรวจสอบ

    ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบายหมายเลขบัตรเครดิต DLP:

  - วีซ่า: ๔๔๘๕๓๖๔๗๓๙๕๒๗๓๕๒
  
  - หมดอายุ: 2/2009

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับ **หมายเลขบัตรเครดิต** ที่จะถูกตรวจพบสำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับของการค้นหาบัตรเครดิต #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  