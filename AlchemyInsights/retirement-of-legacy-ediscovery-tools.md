---
title: เครื่องมือ eDiscovery ดั้งเดิมเกษียณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798568"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>เครื่องมือ eDiscovery ดั้งเดิมเกษียณ

เนื่องจากฟังก์ชัน eDiscovery ใหม่และที่ปรับปรุงแล้วในศูนย์การปฏิบัติตามข้อบังคับของ Microsoft 365 เครื่องมือ eDiscovery ดั้งเดิมและ commandlets ต่อไปนี้จะถูกปลดระวางในเดือนต่อๆ ไป:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [และ In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in-Place ใน Exchange admin center

- cmdlet PowerShell ของ Exchange Online ที่สนับสนุนIn-Place eDiscovery In-Place Holds (cmdlet เหล่านี้จะถูกระบุโดยรวมว่า *-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ต่อไปนี้:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- cmdlet [ของ](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) กล่องจดหมายการค้นหาใน Exchange Online PowerShell
- การดําเนินการต่อไปนี้ใน API ของ Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**ไทม์ไลน์ปลดการเกษียณ**:
- **1 กรกฎาคม 2020** คุณไม่สามารถสร้างการค้นหาและการหยุดใหม่ได้อีกต่อไป แต่คุณสามารถเรียกใช้ แก้ไข และลบการค้นหาที่มีอยู่โดยคุณต้องยอมรับความเสี่ยงของคุณเอง การสนับสนุนของ Microsoft ไม่สนับสนุนIn-Place eDiscovery & Holds ใน EAC อีกต่อไป
    
- **1 ตุลาคม 2020** In-Place & eDiscovery & Holds ใน EAC จะถูกวางในโหมดอ่านอย่างเดียว เพื่อให้คุณสามารถลบการค้นหาและการหยุดที่มีอยู่เท่านั้น

**หากต้องการข้อมูลเพิ่มเติม โปรดดู**:

 - [โยกย้ายการค้นหา eDiscovery ดั้งเดิมและหยุดไปยังศูนย์การปฏิบัติตามข้อบังคับของ Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [การเกษียณเครื่องมือ eDiscovery ดั้งเดิม](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Faq about In-Place eDiscovery and In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



