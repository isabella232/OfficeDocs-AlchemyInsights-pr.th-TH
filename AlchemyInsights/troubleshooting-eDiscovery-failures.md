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
ms.openlocfilehash: b60cfc298ee05375523e3660f407ab03e630c861
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481824"
---
# <a name="troubleshoot-content-search-errors"></a>การแก้ไขปัญหาข้อผิดพลาดการค้นหาเนื้อหา

คุณประสบปัญหาในการค้นหาเนื้อหาหรือล้มเหลวเมื่อคุณส่งออกผลลัพธ์การค้นหาหรือไม่
ตัวอย่างเช่น คุณจะได้รับสิ่งต่อไปนี้เมื่อคุณเรียกใช้การค้นหาหรือไม่

- ข้อผิดพลาด CS007, CS008 หรือ CS012

- ข้อผิดพลาดเซิร์ฟเวอร์ไม่ว่าง/หมดเวลา

- มีข้อผิดพลาดของแอปพลิเคชันเกิดขึ้น

หรือคุณได้รับข้อผิดพลาดการส่งออกเมื่อคุณค้นหาหรือส่งออกผลลัพธ์จากกล่องจดหมายจํานวนมาก (มากกว่า 100,000 รายการ)

For these errors,try the search for the content locations that have failed or update the search by reducing the complexity of the search query. ตัวอย่างเช่น การค้นหาอักขระตัวแทนอาจส่งกลับผลลัพธ์มากเกินไปเพื่อให้ระบบประมวลผล ซึ่งก่อให้เกิดข้อผิดพลาด CS007   

For more information, see [Retry a Content Search to resolve a content location error or](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) [Investigate, troubleshoot, and resolve common eDiscovery issues](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องดาวน์โหลดผลลัพธ์การส่งออก For details, see [Export Content search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
