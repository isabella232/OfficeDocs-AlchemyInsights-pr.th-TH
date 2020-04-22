---
title: ติดตั้ง DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645691"
---
# <a name="setup-dkim"></a>ติดตั้ง DKIM

คําแนะนําที่สมบูรณ์สําหรับการกําหนดค่า DKIM สําหรับโดเมนแบบกําหนดเองใน Microsoft 365[อยู่ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. สําหรับโดเมนที่กําหนดเอง**แต่ละ**โดเมน คุณจะต้องสร้างระเบียน DKIM CNAME**สอง**ระเบียนที่บริการโฮสต์ DNS ของโดเมน (โดยทั่วไปคือ บริษัทจดทะเบียนโดเมน) ตัวอย่างเช่น contoso.comและfourthcoffee.comต้องใช้ระเบียน DKIM CNAME 4 ระเบียน คือ สองระเบียนสําหรับcontoso.comและสองระเบียนสําหรับfourthcoffee.com

   ระเบียน CNAME ของ DKIM**สําหรับแต่ละโดเมน**ที่กําหนดเองใช้รูปแบบต่อไปนี้

   - **ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>คือข้อความทางด้านซ้ายของ`.mail.protection.outlook.com`ระเบียน MX ที่กําหนดเองสําหรับโดเมนแบบกําหนดเอง (ตัวอย่างเช่น`contoso-com`สําหรับโดเมนcontoso.com) \<InitialDomain\>คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสําหรับ Microsoft 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณได้สร้างระเบียน CNAME สําหรับโดเมนแบบกําหนดเองของคุณแล้ว ให้ปฏิบัติตามคําแนะนําต่อไปนี้

   ก.ส. [ลงชื่อเข้าใช้ Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทํางานหรือที่โรงเรียนของคุณ

   B เลือกไอคอนตัวเปิดใช้แอปที่ด้านบนซ้าย แล้วเลือก**ผู้ดูแลระบบ**

   C ในการนําทางด้านซ้ายล่าง ให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**

   D ไปที่**การป้องกัน** > **DKIM**

   ตะวัน ออก เลือกโดเมน แล้วเลือก**เปิดใช้งาน**สําหรับ**เซ็นชื่อข้อความสําหรับโดเมนนี้ด้วยลายเซ็น DKIM** ทําซ้ําขั้นตอนนี้สําหรับแต่ละโดเมนแบบกําหนดเอง
