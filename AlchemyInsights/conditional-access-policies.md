---
title: นโยบายการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 25dc98397920e4fbf28895f5961f154381e11c92
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812278"
---
# <a name="conditional-access-policies"></a>นโยบายการเข้าถึงแบบมีเงื่อนไข

การเข้าถึงตามเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณสามารถบังคับใช้ตัวควบคุมในการเข้าถึงแอปในสภาพแวดล้อมของคุณโดยยึดตามเงื่อนไขที่เฉพาะเจาะจงและมีการจัดการจากตำแหน่งที่ตั้งส่วนกลาง

เรียนรู้เพิ่มเติมเกี่ยวกับการ[เข้าถึงแบบมีเงื่อนไขของ AZURE AD](https://docs.microsoft.com/azure/active-directory/conditional-access/)  

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่21ตุลาคม๒๐๑๙และคุณจะได้รับพร้อมท์สำหรับ MFA โดยไม่คาดคิดคุณอาจมี [ค่าเริ่มต้นของความปลอดภัย](https://aka.ms/securitydefaults) ที่เปิดใช้งานในผู้เช่าของคุณ

**เมื่อต้องการจัดการค่าเริ่มต้นด้านความปลอดภัย**

1. ลงชื่อเข้าใช้ [ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822) ด้วยข้อมูลประจำตัวของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปยัง [คุณสมบัติ Azure active](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)directory

3. ที่ด้านล่างของหน้าให้คลิก**จัดการค่าเริ่มต้นด้านความปลอดภัย**

4. คลิก **ใช่** เพื่อเปิดใช้งานค่าเริ่มต้นของความปลอดภัยหรือ **ไม่ใช่** เพื่อปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย
