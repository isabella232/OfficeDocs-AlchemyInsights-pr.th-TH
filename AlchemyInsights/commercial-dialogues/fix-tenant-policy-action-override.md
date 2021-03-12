---
title: แก้ไขนโยบายผู้เช่า (การแทนที่การแอคชัน)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748986"
---
# <a name="fix-tenant-policy-action-override"></a>แก้ไขนโยบายผู้เช่า (การแทนที่การแอคชัน)

นโยบายการป้องกันสแปมในผู้เช่าของคุณมีผลต่อข้อความนี้ เมื่อต้องการตรวจทานนโยบาย ให้ทต่อไปนี้:

1. ไปที่ศูนย์การรักษา [ความปลอดภัยของ office 365 &การปฏิบัติตาม](https://go.microsoft.com/fwlink/p/?linkid=2077143)นโยบาย จากนั้นไปที่ **การป้องกัน**  >    >  [สแปมนโยบายการจัดการ](https://go.microsoft.com/fwlink/?linkid=2101518)ภัยคุกคาม
2. ตรวจสอบเพื่อดูว่าแหล่งนโยบาย **ระบุถึง** สิ่งต่อไปนี้หรือไม่:  **ข้อความ Add-Xheader/ModifySubject/Redirect/Delete/No action/ ข้อความ BCC**

    ถ้าเป็นดังนั้น **บนแท็บ แบบ** ปรับแต่งเอง ให้ตรวจสอบการตั้งค่าของนโยบายที่ได้รับผลกระทบจากข้อความ อาจเป็นไปได้ว่าการตั้งค่ามาตรฐาน **ที่ปรับใช้** กับลูกค้า Exchange Online Protection ทั้งหมดที่ได้รับผลกระทบจากข้อความ

For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
