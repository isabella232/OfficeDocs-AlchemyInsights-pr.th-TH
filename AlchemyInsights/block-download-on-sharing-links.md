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
# <a name="block-download-on-sharing-links"></a>บล็อกดาวน์โหลดบนลิงก์การแชร์

การ**ดาวน์โหลดบล็อก**จะพร้อมใช้งานสำหรับการ**เชื่อมโยงแบบดูอย่างเดียว**ไปยังเอกสาร Office เมื่อคุณเลือกตัวเลือกนี้บุคคลที่เข้าถึงไฟล์ผ่านลิงก์ที่คุณสร้างขึ้นจะไม่เห็นตัวเลือกในการดาวน์โหลดพิมพ์หรือคัดลอกไฟล์

ผู้ดูแลระบบสามารถควบคุมได้ว่าการตั้งค่า "บล็อกการดาวน์โหลด" ปรากฏขึ้นเฉพาะสำหรับไฟล์ Office หรือไม่โดยการเปลี่ยนการ `BlockDownloadLinksFileType` ตั้งค่าใน Cmdlet [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) หรือตั้งค่าการตั้งค่า [-get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell
