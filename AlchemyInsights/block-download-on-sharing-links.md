---
title: บล็อกดาวน์โหลดบนลิงก์การแชร์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685761"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="fdec2-102">บล็อกดาวน์โหลดบนลิงก์การแชร์</span><span class="sxs-lookup"><span data-stu-id="fdec2-102">Block download on sharing links</span></span>

<span data-ttu-id="fdec2-103">การ**ดาวน์โหลดบล็อก**จะพร้อมใช้งานสำหรับการ**เชื่อมโยงแบบดูอย่างเดียว**ไปยังเอกสาร Office</span><span class="sxs-lookup"><span data-stu-id="fdec2-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="fdec2-104">เมื่อคุณเลือกตัวเลือกนี้บุคคลที่เข้าถึงไฟล์ผ่านลิงก์ที่คุณสร้างขึ้นจะไม่เห็นตัวเลือกในการดาวน์โหลดพิมพ์หรือคัดลอกไฟล์</span><span class="sxs-lookup"><span data-stu-id="fdec2-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="fdec2-105">ผู้ดูแลระบบสามารถควบคุมได้ว่าการตั้งค่า "บล็อกการดาวน์โหลด" ปรากฏขึ้นเฉพาะสำหรับไฟล์ Office หรือไม่โดยการเปลี่ยนการ `BlockDownloadLinksFileType` ตั้งค่าใน Cmdlet [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) หรือตั้งค่าการตั้งค่า [-get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell</span><span class="sxs-lookup"><span data-stu-id="fdec2-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
