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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157740"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม

เป็นผลมาจากฟังก์ชัน eDiscovery ใหม่และปรับปรุงแล้วใน Microsoft ๓๖๕ศูนย์ปฏิบัติตามกฎระเบียบเครื่องมือ eDiscovery แบบดั้งเดิมต่อไปนี้และ commandlets จะถูกยกเลิกในเดือนที่จะมาถึง:

- [ในตำแหน่ง eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)และ[ในตำแหน่ง](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)ที่เก็บอยู่ในศูนย์ดูแลอัตราแลกเปลี่ยน

- Cmdlets PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนที่สนับสนุน eDiscovery ในตำแหน่งและในสถานที่เก็บ (Cmdlets เหล่านี้จะมีการระบุรวมเป็น *-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ของต่อไปนี้:

    - [MailboxSearch ใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [เริ่มต้น-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [หยุด-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [ชุด-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet[กล่องจดหมายค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน
- การดำเนินการต่อไปนี้ใน API บริการเว็บของอัตราแลกเปลี่ยน:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [โปรแกรม Office ๓๖๕ขั้นสูง eDiscovery v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**ระยะเวลาสำหรับการเกษียณอายุ**:
- วันที่1เมษายน๒๐๒๐: คุณจะไม่สามารถสร้างการค้นหาใหม่และเก็บไว้ได้แต่คุณยังสามารถเรียกใช้แก้ไขและลบการค้นหาที่มีอยู่ได้ด้วยความเสี่ยงของคุณเอง ฝ่ายสนับสนุนของ Microsoft จะไม่สนับสนุนในตำแหน่ง eDiscovery & ในแบบ EAC

- 1กรกฎาคม๒๐๒๐: & eDiscovery ในสถานที่เก็บฟังก์ชันในแบบ EAC จะถูกวางในโหมดอ่านอย่างเดียว ซึ่งหมายความว่าคุณจะสามารถลบการค้นหาที่มีอยู่และถือได้

**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:

 - [ย้ายการค้นหา eDiscovery ดั้งเดิมและถือเป็นศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft ๓๖๕](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [คำถามที่พบบ่อยเกี่ยวกับ eDiscovery ในสถานที่และในสถานที่ถือ](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



