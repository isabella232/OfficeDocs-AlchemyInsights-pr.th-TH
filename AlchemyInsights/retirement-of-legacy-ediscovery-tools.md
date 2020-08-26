---
title: การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902639"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม

ผลลัพธ์ของฟังก์ชัน eDiscovery ใหม่และได้รับการปรับปรุงในศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕จะมีการถอนเครื่องมือ eDiscovery และ commandlet ดังต่อไปนี้ในเดือนที่จะมาถึงดังต่อไปนี้

- [EDiscovery ในสถาน](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ที่และ [ในสถานที่ถือ](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ในศูนย์การจัดการ Exchange

- Cmdlet PowerShell ของ Exchange Online ที่สนับสนุน eDiscovery ในสถานที่และในตำแหน่งที่ถือ (Cmdlet เหล่านี้จะมีการระบุเป็น *-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ต่อไปนี้:

    - [MailboxSearch ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [เริ่มต้น-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [หยุด-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [ตั้งค่า-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [กล่องจดหมายการค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ใน Exchange Online PowerShell
- การดำเนินการต่อไปนี้ใน API เว็บเซอร์วิสของ Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [ขั้นสูง eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**ไทม์ไลน์สำหรับการเกษียณอายุ**:
- **1 กรกฎาคม๒๐๒๐** คุณไม่สามารถสร้างการค้นหาใหม่และจัดเก็บได้อีกต่อไปแต่คุณสามารถเรียกใช้แก้ไขและลบการค้นหาที่มีอยู่ได้ด้วยความเสี่ยงของคุณเอง ฝ่ายสนับสนุนของ Microsoft ไม่สนับสนุนการใช้ eDiscovery ในตำแหน่งที่ & อยู่ใน EAC อีกต่อไป
    
- **1 ตุลาคม๒๐๒๐** & eDiscovery ในสถานที่มีฟังก์ชันการทำงานใน EAC จะถูกวางไว้ในโหมดอ่านอย่างเดียวเพื่อให้คุณสามารถเอาการค้นหาที่มีอยู่และการค้นหาที่มีอยู่ออกได้เท่านั้น

**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:

 - [โยกย้ายการค้นหา eDiscovery ดั้งเดิมและถือเป็นศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [คำถามที่ถามบ่อยเกี่ยวกับ eDiscovery ในสถานที่และในสถานที่ถือ](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



