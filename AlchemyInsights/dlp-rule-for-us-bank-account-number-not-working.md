---
title: กฎ DLP สำหรับหมายเลขบัญชีธนาคารของสหรัฐอเมริกาไม่ทำงาน
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679315"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ปัญหา DLP เกี่ยวกับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**ปัญหา DLP เกี่ยวกับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา**

คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขบัญชีธนาคารสหรัฐอเมริกา** เมื่อใช้ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ใน O365 ใช่หรือไม่ ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นสำหรับสิ่งที่นโยบาย DLP กำลังค้นหาเมื่อมีการประเมิน
  
ตัวอย่างเช่นสำหรับนโยบาย **หมายเลขบัญชีธนาคารสหรัฐอเมริกา** ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๘๕% ดังต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์:
  
- **[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** ตัวเลข8-17

- **[ลวดลาย:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ตัวเลขที่ติดต่อกัน

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มี Checksum

- **[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** นโยบาย DLP มีความมั่นใจ๗๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:

  - นิพจน์ทั่วไป Regex_usa_bank_account_number ค้นหาเนื้อหาที่ตรงกับรูปแบบ

  - พบคำสำคัญจาก Keyword_usa_Bank_Account

    ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย **หมายเลขบัญชีธนาคารสหรัฐอเมริกา** : การตรวจสอบบัญชีผู้ใช้๗๘๓๔๔๐๑๑

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับ **หมายเลขบัญชีธนาคารของสหรัฐอเมริกา** ที่จะถูกตรวจพบสำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับสำหรับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  