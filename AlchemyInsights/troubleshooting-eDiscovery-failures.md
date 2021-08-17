---
title: 1490-troubleshooting-eDiscovery-failures
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
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105587"
---
# <a name="troubleshoot-content-search-errors"></a>การแก้ไขปัญหาข้อผิดพลาดการค้นหาเนื้อหา

คุณประสบปัญหาในการค้นหาเนื้อหาหรือล้มเหลวเมื่อคุณส่งออกผลลัพธ์การค้นหาหรือไม่

ตัวอย่างเช่น คุณจะได้รับสิ่งต่อไปนี้เมื่อเรียกใช้การค้นหาหรือไม่

- ข้อผิดพลาด CS008 หรือ CS012

- ข้อผิดพลาดเซิร์ฟเวอร์ไม่ว่าง/หมดเวลา

- มีข้อผิดพลาดของแอปพลิเคชันเกิดขึ้น

หรือเมื่อค้นหาหรือส่งออกผลลัพธ์จากกล่องจดหมายจํานวนมาก (กล่องจดหมายมากกว่า 100,000 กล่อง) คุณได้รับข้อผิดพลาดการส่งออกหรือไม่

For these types of errors, retry the search for the content locations that have failed. [ดู](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)บทความนี้เพื่อดูข้อมูลเพิ่มเติม

ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก: การส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า[100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
