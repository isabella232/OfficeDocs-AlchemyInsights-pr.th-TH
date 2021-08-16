---
title: กล่องจดหมายเก็บถาวรของคุณเกือบเต็มแล้ว
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046771"
---
# <a name="your-archive-mailbox-is-almost-full"></a>กล่องจดหมายเก็บถาวรของคุณเกือบเต็มแล้ว

ถ้าผู้ใช้ได้รับคําเตือน **กล่องจดหมายเก็บถาวรของคุณเกือบเต็ม** แล้ว หรือคุณต้องเพิ่มขนาดของกล่องจดหมายเก็บถาวร ต่อไปนี้คือเคล็ดลับบางอย่าง:

1. ถ้าผู้ใช้ได้รับมอบหมายแผน Exchange Online 1 ให้อัปเกรด **เป็น Exchange Online Plan 2** เพื่อเพิ่มขนาดจาก 50 GB เป็น 100GB
1. ถ้าผู้ใช้ได้รับมอบหมายอย่างใดอย่างหนึ่งต่อไปนี้แล้ว: Exchange Online Plan **2** หรือ Exchange Online Plan 1 ที่มี add-on Exchange Online Archiving ให้ใช้ขั้นตอนด้านล่างเพื่อเปิดใช้งานการเก็บถาวรแบบขยายอัตโนมัติ:
 
    1. [เชื่อมต่อ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. เรียกใช้ commandlet ต่อไปนี้ของผู้ใช้:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. เรียกใช้ commandlet ต่อไปนี้เพื่อยืนยันการเปิดใช้งานให้ผู้ใช้:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

ดูข้อมูลเพิ่มเติมที่:

- [เปิดใช้งานการเก็บถาวรแบบไม่Microsoft 365 - วิธีใช้ของผู้ดูแลระบบ - | เอกสาร Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Onlineจํากัด - รายละเอียดบริการ| เอกสาร Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [อัปเกรดเป็นแผนธุรกิจอื่น| เอกสาร Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

