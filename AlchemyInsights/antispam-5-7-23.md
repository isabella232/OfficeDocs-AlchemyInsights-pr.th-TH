---
title: ป้องกันโรคไข้ - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506462"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>แก้ไขปัญหาการนําส่งอีเมลสําหรับรหัสข้อผิดพลาด 5.7.23

ตรวจสอบระเบียน DNS SPF สําหรับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานแบบสาธารณะบนเว็บ

ตรวจสอบว่า ข้อความขาออกไม่ได้ถูกระบุว่าเป็นสแปม โดย Microsoft และกําหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) ข้อความในพูลการจัดส่งที่มีความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และองค์กรอีเมลปลายทางจะไม่ได้รับการยอมรับ

หากปัญหายังคงมีอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์อีเมลที่คุณกําลังพยายามส่งอีเมล จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดในข้อความตีกลับ การสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้
