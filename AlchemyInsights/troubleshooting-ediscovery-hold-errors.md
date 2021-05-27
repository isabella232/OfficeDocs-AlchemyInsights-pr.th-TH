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
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676285"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>การแก้ไขปัญหา ediscovery มีข้อผิดพลาด

พบปัญหาเกี่ยวกับการหยุด eDiscovery ใช่ไหม ต่อไปนี้เป็นหลักปฏิบัติที่ดีที่สุดบางอย่างที่ควรพิจารณา:

- ตรวจสอบสถานะการกระจายการหยุด  ถ้า สถานะ เป็น **เปิด (รอการรอการ)** **หรือ ปิด (รอ** การค้างอยู่) รอให้การแจกแจงหยุดเสร็จสมบูรณ์
- ผสาน eDiscovery จะหยุดการอัปเดตเป็นคําขอแบบกลุ่มเดียวแทนการอัปเดตนโยบายซ้ําๆ ในแต่ละทรานแซคชัน
- เรียกใช้ Set-CaseHoldPolicy <policyname> -RetryDistribution ใน Powershell ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย For details, see[เชื่อมต่อ to security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).

For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).
For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
