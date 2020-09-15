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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="1296a-102">ไม่มีผลลัพธ์จากการค้นหาเนื้อหา/การส่งออก</span><span class="sxs-lookup"><span data-stu-id="1296a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="1296a-103">ปัญหาเกี่ยวกับการค้นหาเนื้อหา/การส่งออกจะไม่ส่งกลับข้อมูลใดๆอาจเนื่องจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางอย่างที่ตั้งค่าโดยผู้ดูแลระบบที่เฉพาะเจาะจงและไม่สื่อสารกับผู้ดูแลระบบทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="1296a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="1296a-104">เมื่อต้องการแก้ไขปัญหานี้ให้ตรวจสอบดูว่ามีตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบใดที่อาจทำให้เกิดปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="1296a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="1296a-105">เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ Powershell</span><span class="sxs-lookup"><span data-stu-id="1296a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="1296a-106">เรียกใช้ commandlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1296a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="1296a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="1296a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="1296a-108">$Org ComplianceSecurityFilter-องค์กร</span><span class="sxs-lookup"><span data-stu-id="1296a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>