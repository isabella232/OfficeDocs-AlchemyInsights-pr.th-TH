---
title: ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหาเนื้อหา/ส่งออก
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680330"
---
# <a name="no-results-returned-during-content-searchexport"></a>ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหาเนื้อหา/ส่งออก

ถ้าคุณพบปัญหาเกี่ยวกับสถานการณ์สมมติ eDiscovery ดังต่อไปนี้

- การค้นหาเนื้อหา/ส่งออกส่งกลับไม่มีข้อมูลหรือข้อมูลที่ไม่คาดคิด
- การค้นหา eDiscovery หรือการส่งออกล้มเหลว

ปัญหานี้อาจเกิดจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางอย่างที่ตั้งค่าโดยผู้ดูแลระบบที่เฉพาะเจาะจงและไม่มีการสื่อสารกับผู้ดูแลระบบทั้งหมด

เมื่อต้องการแก้ไขปัญหานี้ให้ตรวจสอบว่ามีตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบใดที่อาจทำให้เกิดปัญหาเหล่านี้:

1. เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ Powershell
2. เรียกใช้ commandlet ต่อไปนี้:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบให้ดูที่ [การกรองสิทธิ์สำหรับการค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
