---
title: ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหา/ส่งออกเนื้อหา
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101285"
---
# <a name="no-results-returned-during-content-searchexport"></a>ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหา/ส่งออกเนื้อหา

ถ้าคุณพบปัญหาเกี่ยวกับสถานการณ์ eDiscovery ต่อไปนี้:

- การค้นหา/ส่งออกเนื้อหาไม่ส่งกลับข้อมูลหรือข้อมูลที่ไม่คาดคิด
- การค้นหาหรือการส่งออก eDiscovery ล้มเหลว

ซึ่งอาจเกิดจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางอย่างที่ได้รับการตั้งค่าโดยผู้ดูแลระบบที่ระบุและไม่ได้สื่อสารกับผู้ดูแลระบบทั้งหมด

เมื่อต้องการแก้ไขปัญหานี้ ให้ตรวจสอบว่ามีตัวกรองความปลอดภัยการปฏิบัติตามนโยบายที่อาจทําให้เกิดปัญหาเหล่านี้:

1. เชื่อมต่อ Powershell ของศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย
2. เรียกใช้ commandlets ต่อไปนี้:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
