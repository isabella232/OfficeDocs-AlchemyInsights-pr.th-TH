---
title: ไม่มีผลลัพธ์การค้นหาเนื้อหา
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800650"
---
# <a name="no-results-from-content-searchexports"></a>ไม่มีผลลัพธ์จากเนื้อหาค้นหา/การส่งออก

การตัดสินค้าจากคลังกับเนื้อหาค้นหา/ส่งออกไม่ส่งกลับข้อมูลใด ๆ ที่อาจจะเนื่องจากตัวกรองความปลอดภัยบางปฏิบัติตามกฎระเบียบที่ถูกตั้งค่า โดยผู้ดูแลระบบเฉพาะเจาะจงและไม่สื่อสารกับผู้ดูแลทั้งหมด

การแก้ปัญหานี้ ตรวจสอบเพื่อดูว่า มีตัวกรองความปลอดภัยปฏิบัติตามกฎระเบียบที่อาจทำให้เกิดนี้:
1. เชื่อมต่อกับ Powershell ศูนย์ปฏิบัติตามกฎระเบียบและการรักษาความปลอดภัย
2. เรียกใช้ commandlets ต่อไปนี้:
<br>$org = "yourdomain.com"
<br>รับ-ComplianceSecurityFilter-$org ขององค์กร