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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727242"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="483c9-102">ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหาเนื้อหา/ส่งออก</span><span class="sxs-lookup"><span data-stu-id="483c9-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="483c9-103">ถ้าคุณพบปัญหาเกี่ยวกับสถานการณ์สมมติ eDiscovery ดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="483c9-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="483c9-104">การค้นหาเนื้อหา/ส่งออกส่งกลับไม่มีข้อมูลหรือข้อมูลที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="483c9-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="483c9-105">การค้นหา eDiscovery หรือการส่งออกล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="483c9-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="483c9-106">การดำเนินการนี้อาจเกิดจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบที่ตั้งค่าโดยผู้ดูแลระบบที่เฉพาะเจาะจงและไม่มีการสื่อสารกับผู้ดูแลระบบทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="483c9-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="483c9-107">เมื่อต้องการแก้ไขปัญหานี้ให้ตรวจสอบว่ามีตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบใดที่อาจทำให้เกิดปัญหาเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="483c9-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="483c9-108">เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ Powershell</span><span class="sxs-lookup"><span data-stu-id="483c9-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="483c9-109">เรียกใช้ commandlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="483c9-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="483c9-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบให้ดูที่ [การกรองสิทธิ์สำหรับการค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="483c9-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
