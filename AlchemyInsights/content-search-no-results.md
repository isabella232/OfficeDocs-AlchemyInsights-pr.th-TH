---
title: การค้นหาเนื้อหาไม่มีผลลัพธ์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680666"
---
# <a name="no-results-from-content-searchexports"></a>ไม่มีผลลัพธ์จากการค้นหาเนื้อหา/การส่งออก

ปัญหาเกี่ยวกับการค้นหาเนื้อหา/การส่งออกจะไม่ส่งกลับข้อมูลใดๆอาจเนื่องจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางอย่างที่ตั้งค่าโดยผู้ดูแลระบบที่เฉพาะเจาะจงและไม่สื่อสารกับผู้ดูแลระบบทั้งหมด

เมื่อต้องการแก้ไขปัญหานี้ให้ตรวจสอบดูว่ามีตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบใดที่อาจทำให้เกิดปัญหานี้:
1. เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ Powershell
2. เรียกใช้ commandlet ต่อไปนี้:
<br>$org = "yourdomain.com"
<br>$Org ComplianceSecurityFilter-องค์กร