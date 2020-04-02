---
title: นโยบายการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100639"
---
# <a name="conditional-access-policies"></a>นโยบายการเข้าถึงแบบมีเงื่อนไข

การเข้าถึงแบบมีเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณสามารถบังคับใช้การควบคุมการเข้าถึงแอปในสภาพแวดล้อมของคุณ ทั้งหมดขึ้นอยู่กับเงื่อนไขเฉพาะและจัดการจากตําแหน่งที่ตั้งส่วนกลาง

เรียนรู้เพิ่มเติมเกี่ยวกับ[การเข้าถึงแบบมีเงื่อนไขโฆษณา Azure](https://docs.microsoft.com/azure/active-directory/conditional-access/)  

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์สําหรับ MFA โดยไม่คาดคิด คุณอาจมี[ค่าเริ่มต้นการรักษาความปลอดภัย](http://aka.ms/securitydefaults)ที่เปิดใช้งานในผู้เช่าของคุณโดยไม่คาดคิด

**เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย**

1. ลงชื่อเข้าใช้[ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822)ด้วยข้อมูลประจําตัวของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปที่[คุณสมบัติไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)

3. ที่ด้านล่างของหน้า ให้คลิก**จัดการค่าเริ่มต้นความปลอดภัย**

4. คลิก**ใช่**เพื่อเปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัยหรือ**ไม่ใช่**เพื่อปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัย
