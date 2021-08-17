---
title: การแก้ไขปัญหา ediscovery มีข้อผิดพลาด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1ce8443549ea111bc3ebba9c30c4e621a04926231c24d34c64b6d024194d5249
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886274"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>การแก้ไขปัญหา ediscovery มีข้อผิดพลาด

พบปัญหาเกี่ยวกับการหยุด eDiscovery ใช่ไหม ต่อไปนี้เป็นหลักปฏิบัติที่ดีที่สุดบางอย่างที่ควรพิจารณา:

- ตรวจสอบสถานะการกระจายการหยุด  ถ้าสถานะเป็น **เปิด (รอการพิจารณา)** **หรือ ปิด (รอ** ค้างอยู่) รอให้การแจกแจงหยุดเสร็จสมบูรณ์
- ผสาน eDiscovery จะหยุดการอัปเดตเป็นคําขอแบบกลุ่มเดียวแทนการอัปเดตนโยบายซ้ําๆ กับแต่ละทรานแซคชัน
- เรียกใช้ Set-CaseHoldPolicy <policyname> -RetryDistribution ใน Powershell ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย For details, see[เชื่อมต่อ to security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell).

For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors).
For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
