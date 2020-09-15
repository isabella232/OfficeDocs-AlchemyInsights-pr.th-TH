---
title: การรับรองความถูกต้องแบบหลายปัจจัยที่ไม่คาดคิด
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
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689541"
---
# <a name="unexpected-multi-factor-authentication"></a>การรับรองความถูกต้องแบบหลายปัจจัยที่ไม่คาดคิด

ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่21ตุลาคม๒๐๑๙และคุณจะได้รับพร้อมท์สำหรับ MFA โดยไม่คาดคิดคุณอาจมี [ค่าเริ่มต้นของความปลอดภัย](https://aka.ms/securitydefaults) ที่เปิดใช้งานในผู้เช่าของคุณ 

เมื่อต้องการจัดการค่าเริ่มต้นของความปลอดภัย:

1. ลงชื่อเข้าใช้ [ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822) ด้วยข้อมูลประจำตัวของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปยัง [คุณสมบัติ Azure active](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)directory

3. ที่ด้านล่างของหน้าให้คลิก**จัดการค่าเริ่มต้นด้านความปลอดภัย**

4. คลิก **ใช่** เพื่อเปิดใช้งานค่าเริ่มต้นของความปลอดภัยและ **ไม่** ต้องปิดใช้งานค่าเริ่มต้นของความปลอดภัย
