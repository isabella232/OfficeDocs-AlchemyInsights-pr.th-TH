---
title: ตั้งค่า DKIM ใน Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666283"
---
# <a name="setup-dkim-in-office-365"></a>ตั้งค่า DKIM ใน Office ๓๖๕

คำแนะนำที่สมบูรณ์สำหรับการกำหนดค่า DKIM สำหรับโดเมนที่กำหนดเองใน Office ๓๖๕อยู่ที่[นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. สำหรับ**แต่ละ**โดเมนที่กำหนดเองคุณจำเป็นต้องสร้างระเบียน CNAME แบบ DKIM **2**รายการที่บริการโฮสต์ DNS ของโดเมนของคุณ (โดยทั่วไปคือผู้ลงทะเบียนโดเมน) ตัวอย่างเช่น contoso.com และ fourthcoffee.com ต้องการระเบียน DKIM CNAME สี่เรกคอร์ด: สองสำหรับ contoso.com และสองสำหรับ fourthcoffee.com

   ระเบียน DKIM CNAME สำหรับ**แต่ละ**โดเมนที่กำหนดเองจะใช้รูปแบบต่อไปนี้:

   - **ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`

     **ชี้ไปที่ที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: ๓๖๐๐

   - **ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`

     **ชี้ไปที่ที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: ๓๖๐๐

   \<DomainGUID\>คือข้อความทางด้านซ้ายของ`.mail.protection.outlook.com`ระเบียน MX ที่กำหนดเองสำหรับโดเมนที่กำหนดเอง (ตัว`contoso-com`อย่างเช่นสำหรับโดเมน contoso.com) \<ต้นแบบโด\>เมนคือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสำหรับ Office ๓๖๕ (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณได้สร้างระเบียน CNAME สำหรับโดเมนที่กำหนดเองของคุณแล้วให้ทำตามคำแนะนำต่อไปนี้:

   ราคา . [ลงชื่อเข้าใช้ Office ๓๖๕](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทำงานหรือที่โรงเรียนของคุณ

   B เลือกไอคอนตัวเปิดแอพในด้านบนซ้ายและเลือกผู้**ดูแล**

   C ในการนำทางด้านซ้ายล่างให้ขยายผู้**ดูแล**และเลือก**แลกเปลี่ยน**

   D ไปที่**DKIM**ของ**การป้องกัน** > 

   ตะวัน ออก เลือกโดเมนแล้วเลือก**เปิดใช้งาน**สำหรับ**ข้อความลงชื่อสำหรับโดเมนนี้ด้วยลายเซ็น DKIM** ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนที่กำหนดเอง
