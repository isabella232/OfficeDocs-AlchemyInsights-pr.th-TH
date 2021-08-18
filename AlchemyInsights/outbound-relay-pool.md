---
title: พูลรีเลย์ขาออก
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326096"
---
# <a name="outbound-relay-pool"></a>พูลรีเลย์ขาออก

Microsoft จะเปลี่ยนแปลงการกําหนดค่าบางอย่างเพื่อรีเลย์หรือส่งต่ออีเมลผ่านMicrosoft 365 ข้อความในบางสถานการณ์จะถูกส่งต่อหรือถ่ายทอดผ่านMicrosoft 365โดยใช้พูลรีเลย์พิเศษ ข้อความที่ส่งโดยใช้พูลรีเลย์อาจไปอยู่ในโฟลเดอร์อีเมลขยะของผู้รับ For more information, see [Outbound deliveryพูล](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

เมื่อต้องการหลีกเลี่ยงสถานการณ์โดยใช้พูลรีเลย์ ตรวจสอบให้แน่ใจว่าข้อความที่ส่งต่อ/รีเลย์ตรงกับหนึ่งในเกณฑ์ต่อไปนี้:

- ผู้ส่งขาออกเป็นโดเมนที่ยอมรับของผู้เช่า
- เฟรมเวิร์กนโยบายตรวจสอบผู้ส่ง (Sender Policy Framework - SPF) จะส่งต่อเมื่อข้อความMicrosoft 365เกิดขึ้น
- DomainKeys ที่ระบุจดหมาย (DKIM) บนโดเมนผู้ส่ง P2 จะส่งต่อเมื่อข้อความMicrosoft 365ส่ง
 
ข้อความที่ตรงกับเกณฑ์ด้านบนจะไม่ถูกถ่ายทอดผ่านพูลรีเลย์

ถ้าระเบียน MX ของโดเมนของคุณชี้ไปยังเซิร์ฟเวอร์ของบริษัทอื่นหรือเซิร์ฟเวอร์ภายในองค์กร ให้ใช้การกรองขั้นสูงเพื่อให้แน่ใจว่าการตรวจสอบ SPF ถูกต้องกับอีเมลขาเข้าและหลีกเลี่ยงการส่งอีเมลผ่านพูลรีเลย์

**เราจะรู้ได้อย่างไรว่าเราได้รับผลกระทบจากพูลรีเลย์หรือไม่**

ถ้าอีเมลที่ส่งต่อหรือรีเลย์ของคุณใช้เกณฑ์ใดเกณฑ์หนึ่งข้างต้น ข้อความจะไม่ถ่ายทอดผ่านพูลรีเลย์ อย่างไรก็ตาม ถ้าข้อความถูกส่งผ่านพูลรีเลย์ IP เซิร์ฟเวอร์ขาออกจะอยู่ในช่วง 40.95.0.0/16 และชื่อเซิร์ฟเวอร์ขาออกจะรวม **rly** ในชื่อ

