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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750598"
---
# <a name="fix-connection-policy"></a>แก้ไขนโยบายการเชื่อมต่อ

อีเมลถูกเครื่องหมายว่าปลอดภัยและส่งไปยังกล่องจดหมายเข้าของผู้ใช้เนื่องจากที่อยู่ IP ของผู้ส่งถูกเครื่องหมายว่าปลอดภัยในนโยบายตัวกรองการเชื่อมต่อ เมื่อต้องการตรวจทานนโยบาย ให้ทต่อไปนี้:

1. ไปที่ศูนย์การรักษา [ความปลอดภัยของ office 365 &การปฏิบัติตาม](https://go.microsoft.com/fwlink/p/?linkid=2077143)นโยบาย จากนั้นไปที่ **การป้องกัน**  >    >  [สแปมนโยบายการจัดการ](https://go.microsoft.com/fwlink/?linkid=2101518)ภัยคุกคาม
2. บนแท็บ **แบบ** ปรับแต่งเอง **ให้เลือกนโยบาย** ตัวกรองการเชื่อมต่อ **แล้วเลือก แก้ไข** นโยบาย
3. รีวิว **รายการอนุญาต IP** ดูว่า **มีการเปิดใช้งานรายการ** Safe หรือไม่

    > [!NOTE]
    > Microsoft สมัครใช้งานกับแหล่งข้อมูลของบริษัทอื่นของผู้ส่งที่เชื่อถือได้ ถ้า **เปิดใช้งาน** รายการที่ปลอดภัย ผู้ส่งที่เชื่อถือได้เหล่านี้จะไม่ถูกระบุว่าเป็นสแปมโดยไม่ได้ตั้งใจ ฉันแนะให้เลือกตัวเลือกนี้ เนื่องจากตัวเลือกนี้จะลดจํานวนบวกที่ผิด (จดหมายที่ดีที่จัดประเภทเป็นสแปม) ที่คุณได้รับ
