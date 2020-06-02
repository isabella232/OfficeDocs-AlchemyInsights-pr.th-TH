---
title: การตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509403"
---
# <a name="setup-dkim"></a>การตั้งค่า DKIM

คําแนะนําฉบับสมบูรณ์สําหรับการกําหนดค่า DKIM สําหรับโดเมนแบบกําหนดเองใน Microsoft 365[อยู่ที่นี่](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. สําหรับโดเมนที่กําหนดเอง**แต่ละ**โดเมน คุณจะต้องสร้างระเบียน DKIM CNAME**สอง**รายการที่บริการโฮสต์ DNS ของโดเมน (โดยทั่วไปแล้ว ตัวอย่างเช่น contoso.com และfourthcoffee.comต้องการระเบียน DKIM CNAME สี่รายการ ได้แก่ สองสําหรับcontoso.comและสองสําหรับfourthcoffee.com

   ระเบียน CNAME DKIM**สําหรับแต่ละโดเมน**แบบกําหนดเองใช้รูปแบบต่อไปนี้:

   - **ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่าชี้ถึง**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่าชี้ถึง**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>ข้อความทางด้านซ้ายของระเบียน MX `.mail.protection.outlook.com` ที่กําหนดเองสําหรับโดเมนแบบกําหนดเอง (ตัวอย่างเช่น `contoso-com` สําหรับโดเมนcontoso.com) \<InitialDomain\>คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสําหรับ Microsoft 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณสร้างระเบียน CNAME สําหรับโดเมนแบบกําหนดเองแล้ว ให้ทําตามคําแนะนําต่อไปนี้:

   a. [ลงชื่อเข้าใช้ Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทํางานหรือโรงเรียนของคุณ

   b. เลือกไอคอนตัวเปิดใช้แอปที่ด้านซ้ายบน แล้วเลือก**ผู้ดูแลระบบ**

   c. ในการนําทางด้านซ้ายล่าง ให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**

   D ไปที่**Protection**  >  **DKIM**การป้องกัน

   ตะวัน ออก เลือกโดเมน แล้วเลือก**เปิดใช้งาน**สําหรับ**ข้อความลงชื่อ สําหรับโดเมนนี้ด้วยลายเซ็น DKIM** ทําซ้ําขั้นตอนนี้สําหรับแต่ละโดเมนแบบกําหนดเอง
