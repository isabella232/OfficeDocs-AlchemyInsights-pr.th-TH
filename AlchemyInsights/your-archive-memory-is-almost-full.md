---
title: กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974666"
---
# <a name="your-archive-mailbox-is-almost-full"></a>กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด

ถ้าผู้ใช้ได้รับคำเตือน **กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด** หรือคุณจำเป็นต้องเพิ่มขนาดของกล่องจดหมายเก็บถาวรต่อไปนี้คือเคล็ดลับบางประการ:

1. ถ้าผู้ใช้ได้รับมอบหมายให้มี Exchange Online Plan 1 ให้อัปเกรดเป็นสิทธิ์การใช้งาน **Exchange Online plan 2** เพื่อเพิ่มขนาดจาก๕๐กิกะไบต์ถึง100gb
1. ถ้าผู้ใช้ได้รับมอบหมายอย่างใดอย่างหนึ่งต่อไปนี้: **Exchange Online plan 2** หรือ Exchange online plan 1 ที่มี Add-on ของ exchange Online ที่เก็บถาวรให้ใช้ขั้นตอนด้านล่างนี้เพื่อเปิดใช้งานการเก็บถาวรแบบขยายโดยอัตโนมัติ:
 
    1. [เชื่อมต่อกับ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. เรียกใช้ commandlet ต่อไปนี้สำหรับผู้ใช้:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. เรียกใช้ commandlet ต่อไปนี้เพื่อยืนยันว่ามีการเปิดใช้งานสำหรับผู้ใช้:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

สำหรับข้อมูลเพิ่มเติมให้ดูที่:

- [ เปิดใช้งานการเก็บถาวรแบบไม่จำกัด-วิธีใช้สำหรับผู้ดูแลระบบ-Microsoft ๓๖๕การปฏิบัติตามข้อบังคับ | Microsoft เอกสาร](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [ข้อจำกัดของ Exchange Online-คำอธิบายบริการ | Microsoft เอกสาร](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [อัปเกรดเป็นแผนธุรกิจที่แตกต่างกัน Microsoft เอกสาร](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

