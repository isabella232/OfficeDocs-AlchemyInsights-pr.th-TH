---
title: การตั้งค่า DKIM ใน Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765495"
---
# <a name="setup-dkim-in-office-365"></a>การตั้งค่า DKIM ใน Office 365

คำแนะนำทั้งหมดสำหรับการกำหนดค่า DKIM สำหรับโดเมนที่กำหนดเองใน Office 365 อยู่[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. สำหรับ**แต่ละ**โดเมนที่กำหนดเอง คุณต้องสร้าง**สอง**ระเบียน DKIM CNAME ในโดเมนของคุณโฮสต์บริการ DNS (โดยปกติ โดเมนผู้ลงทะเบียน) ตัวอย่างเช่น contoso.com และ fourthcoffee.com จำเป็นต้องมีระเบียน DKIM CNAME สี่: สำหรับ contoso.com และอีกสองเรือนสำหรับ fourthcoffee.com สองครั้ง

   ระเบียน DKIM CNAME สำหรับ**แต่ละ**โดเมนที่กำหนดเองใช้รูปแบบต่อไปนี้:

   - **ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`

     **ชี้ไปยังที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`

     **ชี้ไปยังที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>คือข้อความที่ด้านซ้ายของ`.mail.protection.outlook.com`ในเรกคอร์ด MX แบบกำหนดเองสำหรับโดเมนกำหนดเอง (ตัวอย่างเช่น`contoso-com`สำหรับ contoso.com โดเมน) \<InitialDomain\>คือโดเมนคุณใช้เมื่อคุณลงทะเบียนไว้สำหรับ Office 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)

2. หลังจากที่คุณสร้างระเบียน CNAME สำหรับโดเมนของคุณเอง ทำคำแนะนำต่อไปนี้:

   อยู่ [ลงชื่อเข้าใช้ Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีของคุณทำงาน หรือที่โรงเรียน

   b เลือกไอคอนตัวเปิดใช้โปรแกรมประยุกต์ในด้านบนซ้าย และเลือก**Admin**

   c ในการนำทางด้านล่างซ้าย ขยาย**Admin**และ**อัตราแลกเปลี่ยน**ที่เลือก

   d ไปที่**การป้องกัน** > **DKIM**

   e เลือกโดเมน และจากนั้น เลือก**เปิดใช้งาน**สำหรับ**ข้อความการเข้าสู่ระบบสำหรับโดเมนนี้มีลายเซ็น DKIM** ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนที่กำหนดเอง
