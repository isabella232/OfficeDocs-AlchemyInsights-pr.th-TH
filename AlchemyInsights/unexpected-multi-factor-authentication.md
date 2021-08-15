---
title: การรับรองความถูกต้องโดยใช้หลายปัจจัยที่ไม่คาดคิด
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: d2b97175049bd9732b7444b029f7ea8610c3d5a2c02878ec5f20ded916baadd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53991158"
---
# <a name="unexpected-multi-factor-authentication"></a>การรับรองความถูกต้องโดยใช้หลายปัจจัยที่ไม่คาดคิด

ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์โดยไม่คาดคิดเกี่ยวกับ MFA คุณอาจเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัยในผู้[](https://aka.ms/securitydefaults)เช่าของคุณ 

เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย:

1. ลงชื่อเข้าใช้ศูนย์การจัดการ [ด้วยข้อมูล](https://go.microsoft.com/fwlink/p/?linkid=834822) รับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปที่[Azure Active Directoryคุณสมบัติ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)

3. ที่ด้านล่างของหน้า ให้คลิก **จัดการค่าเริ่มต้นความปลอดภัย**

4. คลิกใช่ เพื่อเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย **และ** ไม่ใช่ เพื่อปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย
