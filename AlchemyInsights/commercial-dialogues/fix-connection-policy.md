---
title: แก้ไขนโยบายการเชื่อมต่อ
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314863"
---
# <a name="fix-connection-policy"></a>แก้ไขนโยบายการเชื่อมต่อ

อีเมลถูกเครื่องหมายว่าปลอดภัยและส่งไปยังกล่องจดหมายเข้าของผู้ใช้ เนื่องจากที่อยู่ IP ต้นทางถูกเครื่องหมายว่าปลอดภัยในนโยบายตัวกรองการเชื่อมต่อเริ่มต้น เมื่อต้องการตรวจสอบนโยบาย ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ในพอร์ทัล Microsoft 365 Defender ไปที่ <https://security.microsoft.com/> นโยบาย **การ&ร่วมกัน** \> **ทางอีเมล &นโยบาย** \> **ภัยคุกคาม** \> ในส่วน นโยบาย

   เมื่อต้องการไปที่หน้า **นโยบายป้องกันสแปม** <https://security.microsoft.com/antispam> โดยตรง ให้ใช้

2. บนหน้า **นโยบายการป้องกันสแปม** ให้เลือกนโยบายที่ชื่อว่า **นโยบายตัวกรอง** การเชื่อมต่อ (ค่าเริ่มต้น) โดยการคลิกที่ชื่อของนโยบาย

3. ในเส้นปลิวรายละเอียดที่ปรากฏขึ้น ให้คลิก **แก้ไขนโยบาย** ตัวกรองการเชื่อมต่อ **ในส่วน การกรอง** การเชื่อมต่อ

4. รีวิวรายการในส่วน อนุญาต **ข้อความจาก** ที่อยู่ IP หรือช่วงที่อยู่ต่อไปนี้เสมอ และดูว่า **มีการเลือก เปิดใช้งานรายการปลอดภัย** ไว้หรือไม่

   **หมายเหตุ**: Microsoft สมัครใช้งานแหล่งข้อมูลของบริษัทอื่นของผู้ส่งที่เชื่อถือได้ ถ้าเปิดใช้งานรายการที่ปลอดภัย ผู้ส่งที่เชื่อถือได้เหล่านี้จะไม่ถูกระบุว่าเป็นสแปมโดยไม่ได้ตั้งใจ เราขอแนะให้เลือกตัวเลือกนี้ เนื่องจากตัวเลือกนี้จะลดจํานวนบวกที่ผิด (จดหมายที่ดีที่จัดประเภทเป็นสแปม) ที่คุณได้รับ

For more information, see [Configure connection filtering](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
