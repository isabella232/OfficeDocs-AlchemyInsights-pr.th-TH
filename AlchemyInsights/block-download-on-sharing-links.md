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
# <a name="block-download-on-sharing-links"></a>บล็อกการดาวน์โหลดในลิงก์การแชร์

**บล็อกการดาวน์โหลด**จะพร้อมใช้งานสําหรับ**การเชื่อมโยงแบบดูเท่านั้น**ไปยังเอกสาร Office เมื่อคุณเลือกตัวเลือกนี้ บุคคลที่สามารถเข้าถึงไฟล์ผ่านลิงก์ที่คุณสร้างจะไม่เห็นตัวเลือกในการดาวน์โหลด พิมพ์ หรือคัดลอกแฟ้ม

ผู้ดูแลระบบสามารถควบคุมว่าการตั้งค่า "บล็อกดาวน์โหลด" ปรากฏขึ้นเฉพาะสําหรับแฟ้ม Office หรือไม่ โดยการเปลี่ยนแปลง `BlockDownloadLinksFileType` การตั้งค่าใน cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps)หรือ[ตั้งค่า SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell
