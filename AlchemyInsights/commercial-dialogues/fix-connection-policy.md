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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988231"
---
# <a name="fix-connection-policy"></a>แก้ไขนโยบายการเชื่อมต่อ

อีเมลถูกเครื่องหมายว่าปลอดภัยและส่งไปยังกล่องจดหมายเข้าของผู้ใช้ เนื่องจากที่อยู่ IP ของผู้ส่งถูกเครื่องหมายว่าปลอดภัยในนโยบายตัวกรองการเชื่อมต่อ เมื่อต้องการตรวจทานนโยบาย ให้ทต่อไปนี้:

1. ไปที่ศูนย์ [Office 365การรักษา&การปฏิบัติตาม](https://go.microsoft.com/fwlink/p/?linkid=2077143)นโยบายของคุณ แล้วไปที่ **นโยบาย** การจัดการภัยคุกคาม  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518)
2. บนแท็บ **แบบ** ปรับแต่งเอง **ให้เลือกนโยบาย** ตัวกรอง การเชื่อมต่อ แล้วเลือก **แก้ไข** นโยบาย
3. รีวิว **รายการการอนุญาต IP** ดูว่า **รายการตู้เซฟถูก** เปิดใช้งานหรือไม่

    > [!NOTE]
    > Microsoft สมัครใช้งานแหล่งข้อมูลของบริษัทอื่นของผู้ส่งที่เชื่อถือได้ ถ้า **ตู้เซฟ** ถูกเปิดใช้งาน ผู้ส่งที่เชื่อถือได้เหล่านี้จะไม่ถูกระบุว่าเป็นสแปมโดยไม่ได้ตั้งใจ ฉันแนะให้เลือกตัวเลือกนี้ เนื่องจากตัวเลือกนี้จะลดจํานวนบวกที่ผิด (จดหมายที่ดีที่จัดประเภทเป็นสแปม) ที่คุณได้รับ
