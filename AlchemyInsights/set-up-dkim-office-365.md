---
title: ตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808726"
---
# <a name="setup-dkim"></a>ตั้งค่า DKIM

คำแนะนำที่สมบูรณ์สำหรับการกำหนดค่า DKIM สำหรับโดเมนแบบกำหนดเองใน Microsoft ๓๖๕อยู่[ที่นี่](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. สำหรับ **แต่ละ** โดเมนแบบกำหนดเองคุณจะต้องสร้างระเบียน CNAME ของ DKIM **สอง** ระเบียนที่บริการโฮสต์ DNS ของโดเมนของคุณ (โดยทั่วไปคือบริษัทจดทะเบียนโดเมน) ตัวอย่างเช่น contoso.com และ fourthcoffee.com จำเป็นต้องมีระเบียน CNAME ของ DKIM สี่ระเบียน: สองสำหรับ contoso.com และสองสำหรับ fourthcoffee.com

   ระเบียน CNAME ของ DKIM สำหรับ **แต่ละ** โดเมนแบบกำหนดเองจะใช้รูปแบบต่อไปนี้:

   - **ชื่อโฮสต์**: `selector1._domainkey.<CustomDomain>`

     **ชี้ไปยังที่อยู่หรือค่า**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: ๓๖๐๐

   - **ชื่อโฮสต์**: `selector2._domainkey.<CustomDomain>`

     **ชี้ไปยังที่อยู่หรือค่า**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: ๓๖๐๐

   \<DomainGUID\> เป็นข้อความทางด้านซ้ายของ `.mail.protection.outlook.com` ระเบียน MX ที่กำหนดเองสำหรับโดเมนแบบกำหนดเอง (ตัวอย่างเช่น `contoso-com` สำหรับโดเมน contoso.com) \<InitialDomain\> โดเมนที่คุณใช้เมื่อคุณลงชื่อเข้าใช้ Microsoft ๓๖๕ (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณได้สร้างระเบียน CNAME สำหรับโดเมนแบบกำหนดเองของคุณแล้วให้ทำตามคำแนะนำต่อไปนี้:

   a. [ลงชื่อเข้าใช้ Microsoft ๓๖๕](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ด้วยบัญชีผู้ใช้ของที่ทำงานหรือที่โรงเรียนของคุณ

   b. เลือกไอคอนตัวเปิดใช้งานแอปที่มุมบนซ้ายแล้วเลือก**ผู้ดูแลระบบ**

   c. ในการนำทางด้านซ้ายล่างให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**

   d. ไปที่การ**ป้องกัน**  >  **DKIM**

   e. เลือกโดเมนแล้วเลือก**เปิดใช้งาน**สำหรับการ**เซ็นชื่อข้อความสำหรับโดเมนนี้กับลายเซ็น DKIM** ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนแบบกำหนดเอง
