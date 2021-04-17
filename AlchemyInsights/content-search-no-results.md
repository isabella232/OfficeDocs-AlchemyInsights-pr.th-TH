---
title: การค้นหาเนื้อหาไม่มีผลลัพธ์การค้นหา
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816867"
---
# <a name="no-results-from-content-searchexports"></a>ไม่มีผลลัพธ์จากการค้นหา/ส่งออกเนื้อหา

ปัญหาเกี่ยวกับการค้นหา/การส่งออกเนื้อหาไม่ส่งกลับข้อมูลใดๆ อาจเป็นเพราะตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางตัวที่ตั้งค่าโดยผู้ดูแลระบบที่ระบุ และไม่ได้สื่อสารกับผู้ดูแลระบบทั้งหมด

เมื่อต้องการแก้ไขปัญหานี้ ให้ตรวจสอบเพื่อดูว่ามีตัวกรองความปลอดภัยการปฏิบัติตามนโยบายที่อาจเป็นสาเหตุของสิ่งนี้:
1. เชื่อมต่อกับ Powershell ของศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย
2. เรียกใช้ commandlets ต่อไปนี้:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -องค์กร $org