---
title: แอนตี้สแปม-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717344"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>แก้ไขปัญหาการนำส่งอีเมลสำหรับรหัสข้อผิดพลาด5.7.23

ตรวจสอบระเบียน DNS ของ SPF สำหรับโดเมนของคุณที่มีตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานสาธารณะบนเว็บ

ตรวจสอบว่าข้อความขาออกจะไม่ถูกระบุว่าเป็นสแปมโดย Microsoft และกำหนดเส้นทางผ่านทางกลุ่มการนำ[ส่งความเสี่ยงสูง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) ข้อความในกลุ่มการนำส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจึงไม่ได้รับการยอมรับจากองค์กรอีเมลของปลายทาง

ถ้าปัญหายังคงมีอยู่คุณอาจจำเป็นต้องติดต่อผู้ดูแลระบบของ host mail ที่คุณกำลังพยายามส่งอีเมล จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่พร้อมใช้งานในข้อความตีกลับ ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้
