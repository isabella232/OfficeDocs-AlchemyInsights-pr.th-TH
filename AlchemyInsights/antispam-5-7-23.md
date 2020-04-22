---
title: ป้องกันสแปม - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676516"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>แก้ไขปัญหาการนําส่งอีเมลสําหรับรหัสข้อผิดพลาด 5.7.23

ตรวจสอบระเบียน Dns SPF สําหรับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่มีอยู่สาธารณะบนเว็บ

ตรวจสอบว่า ข้อความขาออกไม่ได้ถูกระบุว่าเป็นสแปมโดย Microsoft และกําหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages) ข้อความในพูลการส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจะไม่ได้รับการยอมรับโดยองค์กรอีเมลปลายทาง

หากปัญหายังคงมีอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์อีเมลที่คุณกําลังพยายามส่งอีเมล จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่มีอยู่ในข้อความตีกลับ ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้
