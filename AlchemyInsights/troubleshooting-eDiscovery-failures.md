---
title: ๑๔๙๐-การแก้ไขปัญหา-eDiscovery-ความล้มเหลว
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277834"
---
# <a name="troubleshoot-content-search-errors"></a>การแก้ไขปัญหาข้อผิดพลาดในการค้นหาเนื้อหา

คุณพบปัญหาเกี่ยวกับการค้นหาเนื้อหาหรือความล้มเหลวเมื่อคุณส่งออกผลลัพธ์การค้นหาหรือไม่

ตัวอย่างเช่นคุณจะได้รับสิ่งต่อไปนี้เมื่อเรียกใช้การค้นหา

- ข้อผิดพลาด CS008 หรือ CS012

- ข้อผิดพลาดของเซิร์ฟเวอร์ไม่ว่าง/หมดเวลา

- เกิดข้อผิดพลาดของแอปพลิเคชัน

หรือเมื่อการค้นหาหรือส่งออกผลลัพธ์จากกล่องจดหมายจำนวนมาก (มากกว่ากล่องจดหมาย๑๐๐,๐๐๐) คุณจะได้รับข้อผิดพลาดในการส่งออกหรือไม่

สำหรับข้อผิดพลาดชนิดเหล่านี้ให้ลองค้นหาตำแหน่งที่ตั้งเนื้อหาที่ล้มเหลว ดู  [บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) สำหรับข้อมูลเพิ่มเติม

ถ้าคุณกำลังส่งออกกล่องจดหมายมากกว่า100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก:[ส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
