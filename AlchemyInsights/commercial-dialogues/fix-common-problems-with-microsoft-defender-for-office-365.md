---
title: แก้ไขปัญหาทั่วไปเกี่ยวกับ Microsoft Defender Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330079"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>แก้ไขปัญหาทั่วไปเกี่ยวกับ Microsoft Defender Office 365

ต่อไปนี้เป็นวิธีแก้ไขปัญหาทั่วไปบางอย่างของ Microsoft Defender Office 365:

- **การหน่วงเวลาข้อความ**:

  ความล่าช้าในการส่งอีเมลอาจเกิดจากตู้เซฟที่สแกนข้อความ For more information, see[ตู้เซฟ Attachments policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **รายงานผลลัพธ์ที่เป็นบวกหรือลบที่ผิด**:

  ดูข้อมูลเพิ่มเติมที่[รายงานข้อความและไฟล์ไปยัง Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **เปิดใช้งานการป้องกันตู้เซฟลิงก์:**

  1. ในMicrosoft 365 Defenderที่ <https://security.microsoft.com/> ให้ไปที่ นโยบาย **&การ&** \> **ร่วมกันทางอีเมล ตู้เซฟ** \>  \> **นโยบายภัยคุกคาม** ในส่วน นโยบาย

     เมื่อต้องการไปยังหน้า **ตู้เซฟลิงก์** ของคุณ <https://security.microsoft.com/safelinksv2> โดยตรง ให้ใช้

  2. บนหน้า **ตู้เซฟ** ลิงก์ของคุณ ให้เลือกนโยบายโดยการคลิกที่ชื่อของนโยบาย
  3. ในรายละเอียดที่ปรากฏขึ้น ให้เลือกปฏิบัติตามขั้นตอนใดขั้นตอนหนึ่งต่อไปนี้
     - เมื่อต้องการเพิ่มนโยบายใหม่ ให้เลือก **+** สร้าง ตัวช่วยสร้างจะเปิดใช้งานเพื่อช่วยให้คุณกําหนดการตั้งค่านโยบายของคุณ
     - เมื่อต้องการแก้ไขนโยบายที่มีอยู่ ให้เลือกนโยบายโดยการคลิกที่ชื่อของนโยบาย ในส่วนเมนูปลิวรายละเอียดที่ปรากฏขึ้น **ให้เลือก** แก้ไข **ในส่วนการตั้งค่า** การป้องกัน
  4. บนหน้า **การตั้งค่าการป้องกัน** ให้กําหนดค่าการตั้งค่าต่อไปนี้
     - เปิด **เลือกการแอคชันของ URL ที่อาจเป็นอันตรายที่ไม่รู้จักใน** ข้อความ
     - เลือก **ใช้ลิงก์ที่ปลอดภัยกับข้อความที่ส่งภายใน** องค์กร

  ดูข้อมูลเพิ่มเติมที่ ตั้งค่า[นโยบายตู้เซฟลิงก์ใน Microsoft Defender Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
