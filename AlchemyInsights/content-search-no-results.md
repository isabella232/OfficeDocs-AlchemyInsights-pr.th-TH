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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="242c6-102">ไม่มีผลลัพธ์จากการค้นหา/ส่งออกเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="242c6-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="242c6-103">ปัญหาเกี่ยวกับการค้นหา/การส่งออกเนื้อหาไม่ส่งกลับข้อมูลใดๆ อาจเป็นเพราะตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางตัวที่ตั้งค่าโดยผู้ดูแลระบบที่ระบุ และไม่ได้สื่อสารกับผู้ดูแลระบบทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="242c6-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="242c6-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ตรวจสอบเพื่อดูว่ามีตัวกรองความปลอดภัยการปฏิบัติตามนโยบายที่อาจเป็นสาเหตุของสิ่งนี้:</span><span class="sxs-lookup"><span data-stu-id="242c6-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="242c6-105">เชื่อมต่อกับ Powershell ของศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="242c6-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="242c6-106">เรียกใช้ commandlets ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="242c6-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="242c6-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="242c6-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="242c6-108">Get-ComplianceSecurityFilter -องค์กร $org</span><span class="sxs-lookup"><span data-stu-id="242c6-108">Get-ComplianceSecurityFilter -Organization $org</span></span>