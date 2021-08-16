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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058021"
---
# <a name="no-results-from-content-searchexports"></a>ไม่มีผลลัพธ์จากการค้นหา/ส่งออกเนื้อหา

ปัญหาเกี่ยวกับการค้นหา/การส่งออกเนื้อหาไม่ส่งกลับข้อมูลใดๆ อาจเป็นเพราะตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางตัวที่ตั้งค่าโดยผู้ดูแลระบบที่ระบุ และไม่ได้สื่อสารกับผู้ดูแลระบบทั้งหมด

เมื่อต้องการแก้ไขปัญหานี้ ให้ตรวจสอบเพื่อดูว่ามีตัวกรองความปลอดภัยการปฏิบัติตามนโยบายที่อาจเป็นสาเหตุของสิ่งนี้:
1. เชื่อมต่อ Powershell ของศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย
2. เรียกใช้ commandlets ต่อไปนี้:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -องค์กร $org