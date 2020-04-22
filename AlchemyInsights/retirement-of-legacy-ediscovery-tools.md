---
title: การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650587"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม

จากฟังก์ชัน eDiscovery ใหม่ ที่ได้รับการปรับปรุงในศูนย์การปฏิบัติตามกฎระเบียบ 365 Microsoft เครื่องมือ eDiscovery แบบดั้งเดิมและ commandlets ต่อไปนี้จะออกใช้ในเดือนที่จะมาถึง:

- การหยุดพักในสถานที่[eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)และ[ในสถานที่](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)ในศูนย์การจัดการ Exchange

- Cmdlet แบบออนไลน์ของอัตราแลกเปลี่ยนที่สนับสนุน eDiscovery ในสถานที่และในสถานที่ (cmdlet เหล่านี้ถูกระบุรวมเป็น cmdlet กล่องจดหมาย Search) ซึ่งรวมถึง cmdlet ต่อไปนี้:

    - [กล่องจดหมายใหม่ค้นหา](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [กล่องจดหมายเริ่มต้นค้นหา](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [หยุดการค้นหากล่องจดหมาย](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [ตั้งค่ากล่องจดหมายค้นหา](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- คําสั่งจัดการ[กล่องจดหมายการค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน
- การดําเนินการต่อไปนี้ใน API บริการเว็บอัตราแลกเปลี่ยน:
    - [รับกล่องจดหมายที่ค้นหาได้](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [ตั้งค่าการระงับบนกล่องจดหมาย](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [การฝากข้อความ](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [ขั้นสูง eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**ระยะเวลาเกษียณ :**
- 1 เมษายน 2020: คุณจะไม่สามารถสร้างการค้นหาและการระงับใหม่ได้ แต่คุณยังสามารถเรียกใช้ แก้ไข และลบการค้นหาที่มีอยู่ตามความเสี่ยงของคุณเองได้ ฝ่ายสนับสนุนของ Microsoft จะไม่สนับสนุน & eDiscovery ในตําแหน่งใน EAC อีกต่อไป

- 1 กรกฎาคม 2020: & eDiscovery ในสถานที่เก็บใน EAC จะถูกวางในโหมดอ่านอย่างเดียว ซึ่งหมายความว่าคุณจะสามารถลบการค้นหาที่มีอยู่และระงับได้เท่านั้น

**สําหรับข้อมูลเพิ่มเติม โปรดดูที่**:

 - [โยกย้ายการค้นหา eDiscovery ดั้งเดิมและระงับไปยังศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [คําถามที่พบบ่อยเกี่ยวกับ อิน-เพลส](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



