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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516798"
---
# <a name="no-results-from-content-searchexports"></a>ไม่มีผลลัพธ์จากเนื้อหาค้นหา/การส่งออก

การตัดสินค้าจากคลังกับเนื้อหาค้นหา/ส่งออกไม่ส่งกลับข้อมูลใด ๆ ที่อาจจะเนื่องจากตัวกรองความปลอดภัยบางปฏิบัติตามกฎระเบียบที่ถูกตั้งค่า โดยผู้ดูแลระบบเฉพาะเจาะจงและไม่สื่อสารกับผู้ดูแลทั้งหมด

การแก้ปัญหานี้ ตรวจสอบเพื่อดูว่า มีตัวกรองความปลอดภัยปฏิบัติตามกฎระเบียบที่อาจทำให้เกิดนี้:
1. เชื่อมต่อกับ Powershell ศูนย์ปฏิบัติตามกฎระเบียบและการรักษาความปลอดภัย
2. เรียกใช้ commandlets ต่อไปนี้:
<br>$org = "yourdomain.com"
<br>รับ-ComplianceSecurityFilter-$org ขององค์กร