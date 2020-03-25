---
title: การรับรองความถูกต้องด้วยหลายปัจจัยที่ไม่คาดคิด
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946852"
---
# <a name="unexpected-multi-factor-authentication"></a>การรับรองความถูกต้องด้วยหลายปัจจัยที่ไม่คาดคิด

ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์สําหรับ MFA โดยไม่คาดคิด คุณอาจมี[ค่าเริ่มต้นการรักษาความปลอดภัย](http://aka.ms/securitydefaults)ที่เปิดใช้งานในผู้เช่าของคุณโดยไม่คาดคิด 

เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย:

1. ลงชื่อเข้าใช้[ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822)ด้วยข้อมูลประจําตัวของผู้ดูแลระบบส่วนกลางของคุณ

2. ไปที่[คุณสมบัติไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)

3. ที่ด้านล่างของหน้า ให้คลิก**จัดการค่าเริ่มต้นความปลอดภัย**

4. คลิก**ใช่**เพื่อเปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัยและ**ไม่ใช่**เพื่อปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัย
