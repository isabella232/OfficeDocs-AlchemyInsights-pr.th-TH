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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="6edf8-102">ไม่มีผลลัพธ์จากเนื้อหาค้นหา/การส่งออก</span><span class="sxs-lookup"><span data-stu-id="6edf8-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="6edf8-103">การตัดสินค้าจากคลังกับเนื้อหาค้นหา/ส่งออกไม่ส่งกลับข้อมูลใด ๆ ที่อาจจะเนื่องจากตัวกรองความปลอดภัยบางปฏิบัติตามกฎระเบียบที่ถูกตั้งค่า โดยผู้ดูแลระบบเฉพาะเจาะจงและไม่สื่อสารกับผู้ดูแลทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="6edf8-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="6edf8-104">การแก้ปัญหานี้ ตรวจสอบเพื่อดูว่า มีตัวกรองความปลอดภัยปฏิบัติตามกฎระเบียบที่อาจทำให้เกิดนี้:</span><span class="sxs-lookup"><span data-stu-id="6edf8-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="6edf8-105">เชื่อมต่อกับ Powershell ศูนย์ปฏิบัติตามกฎระเบียบและการรักษาความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="6edf8-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="6edf8-106">เรียกใช้ commandlets ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6edf8-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="6edf8-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="6edf8-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="6edf8-108">รับ-ComplianceSecurityFilter-$org ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="6edf8-108">Get-ComplianceSecurityFilter -Organization $org</span></span>