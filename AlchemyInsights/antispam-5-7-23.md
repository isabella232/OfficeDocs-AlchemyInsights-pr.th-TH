---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932188"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>แก้ไขปัญหาการส่งอีเมลของรหัสข้อผิดพลาด 5.7.23

ตรวจสอบระเบียน DNS ของ SPF กับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานแบบสาธารณะบนเว็บ

ตรวจสอบว่าข้อความขาออกไม่ได้ระบุว่าเป็นสแปมโดยไมโครซอฟท์ และถูกเส้นทางผ่าน [พูลการส่งข้อความความเสี่ยง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)สูง ข้อความในพูลการส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF ดังนั้นจึงไม่ได้รับการยอมรับจากองค์กรอีเมลปลายทาง

ถ้าปัญหายังคงอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์จดหมายที่คุณพยายามส่งอีเมล จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่พร้อมใช้งานในข้อความแจ้งการตีกลับ ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถช่วยเหลือเพิ่มเติมได้
