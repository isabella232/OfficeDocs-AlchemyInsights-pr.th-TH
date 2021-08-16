---
title: นโยบายการเข้าถึงตามเงื่อนไข
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: a518d70f03f3034a60f0c9ded40ee6ab5140a5163021337c3a2aee7f18575c3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033729"
---
# <a name="conditional-access-policies"></a>นโยบายการเข้าถึงตามเงื่อนไข

การเข้าถึงตามเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณบังคับใช้การควบคุมการเข้าถึงแอปในสภาพแวดล้อมของคุณ ทั้งหมดจะยึดตามเงื่อนไขที่เฉพาะเจาะจงและจัดการจากศูนย์กลาง

เรียนรู้เพิ่มเติมเกี่ยวกับ[การเข้าถึงตามเงื่อนไขของ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/)  

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์โดยไม่คาดคิดเกี่ยวกับ MFA คุณอาจเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัยใน [](https://aka.ms/securitydefaults)ผู้เช่าของคุณ

**เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย**

1. ลงชื่อเข้าใช้ศูนย์การจัดการ [ด้วยข้อมูล](https://go.microsoft.com/fwlink/p/?linkid=834822) รับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปที่[Azure Active Directoryคุณสมบัติ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)

3. ที่ด้านล่างของหน้า ให้คลิก **จัดการค่าเริ่มต้นความปลอดภัย**

4. คลิกใช่ เพื่อเปิดใช้งานค่าเริ่มต้นความปลอดภัย **หรือ** ไม่ใช่ เพื่อปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย
