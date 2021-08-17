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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108575"
---
# <a name="setup-dkim"></a>ตั้งค่า DKIM

คําแนะนําที่สมบูรณ์ในการกําหนดค่า DKIM Microsoft 365โดเมนแบบกําหนด[เองใน จะ](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)อยู่ที่นี่

1. For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's hosting service (typically, the domain registrar). ตัวอย่างเช่น contoso.com fourthcoffee.com DKIM CNAME สี่ระเบียน: สองระเบียน contoso.com และสอง fourthcoffee.com สองระเบียน

   ระเบียน DKIM CNAME ของแต่ละ **โดเมน** แบบปรับแต่งเองจะใช้รูปแบบต่อไปนี้:

   - **ชื่อโฮสต์**: `selector1._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่าชี้ไปยัง**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **ชื่อโฮสต์**: `selector2._domainkey.<CustomDomain>`

     **ที่อยู่หรือค่าชี้ไปยัง**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> คือข้อความที่อยู่ทางด้านซ้ายของ `.mail.protection.outlook.com` ในระเบียน MX ที่ปรับแต่งเองของโดเมนแบบ contoso.com `contoso-com` โดเมน) \<InitialDomain\>คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนMicrosoft 365โดเมนของคุณ (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณสร้างระเบียน CNAME ของคุณแล้ว ให้ปฏิบัติตามคําแนะนําต่อไปนี้:

   a. [ลงชื่อเข้าใช้บัญชีMicrosoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)หรือโรงเรียนของคุณ

   b. เลือกไอคอนตัวเปิดใช้แอป ที่มุมบนซ้าย **แล้วเลือก** ผู้ดูแลระบบ

   c. ในการนําทางด้านล่างซ้าย **ให้ขยาย** ผู้ดูแลระบบ แล้วเลือก **Exchange**

   d. ไปที่ **Protection**  >  **DKIM**

   e. เลือกโดเมน แล้วเลือก **เปิดใช้งาน** เพื่อเซ็นชื่อ **ข้อความโดเมนนี้ด้วยลายเซ็น DKIM** ทําซ้ําขั้นตอนนี้กับโดเมนแบบปรับแต่งเองแต่ละโดเมน
