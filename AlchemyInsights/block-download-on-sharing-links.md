---
title: บล็อกการดาวน์โหลดในลิงก์การแชร์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358511"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="b8421-102">บล็อกการดาวน์โหลดในลิงก์การแชร์</span><span class="sxs-lookup"><span data-stu-id="b8421-102">Block download on sharing links</span></span>

<span data-ttu-id="b8421-103">**บล็อกการดาวน์โหลด**จะพร้อมใช้งานสําหรับ**การเชื่อมโยงแบบดูเท่านั้น**ไปยังเอกสาร Office</span><span class="sxs-lookup"><span data-stu-id="b8421-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="b8421-104">เมื่อคุณเลือกตัวเลือกนี้ บุคคลที่สามารถเข้าถึงไฟล์ผ่านลิงก์ที่คุณสร้างจะไม่เห็นตัวเลือกในการดาวน์โหลด พิมพ์ หรือคัดลอกแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="b8421-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="b8421-105">ผู้ดูแลระบบสามารถควบคุมว่าการตั้งค่า "บล็อกดาวน์โหลด" ปรากฏขึ้นเฉพาะสําหรับแฟ้ม Office หรือไม่ โดยการเปลี่ยนแปลง `BlockDownloadLinksFileType` การตั้งค่าใน cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps)หรือ[ตั้งค่า SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell</span><span class="sxs-lookup"><span data-stu-id="b8421-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
