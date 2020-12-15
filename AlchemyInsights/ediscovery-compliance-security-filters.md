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
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="e4361-102">ไม่มีผลลัพธ์ที่ส่งกลับระหว่างการค้นหาเนื้อหา/ส่งออก</span><span class="sxs-lookup"><span data-stu-id="e4361-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="e4361-103">ถ้าคุณพบปัญหาเกี่ยวกับสถานการณ์สมมติ eDiscovery ดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="e4361-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="e4361-104">การค้นหาเนื้อหา/ส่งออกส่งกลับไม่มีข้อมูลหรือข้อมูลที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="e4361-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="e4361-105">การค้นหา eDiscovery หรือการส่งออกล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="e4361-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="e4361-106">ปัญหานี้อาจเกิดจากตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบบางอย่างที่ตั้งค่าโดยผู้ดูแลระบบที่เฉพาะเจาะจงและไม่มีการสื่อสารกับผู้ดูแลระบบทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e4361-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="e4361-107">เมื่อต้องการแก้ไขปัญหานี้ให้ตรวจสอบว่ามีตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบใดที่อาจทำให้เกิดปัญหาเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="e4361-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="e4361-108">เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ Powershell</span><span class="sxs-lookup"><span data-stu-id="e4361-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e4361-109">เรียกใช้ commandlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e4361-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="e4361-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับตัวกรองความปลอดภัยการปฏิบัติตามกฎระเบียบให้ดูที่ [การกรองสิทธิ์สำหรับการค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="e4361-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
