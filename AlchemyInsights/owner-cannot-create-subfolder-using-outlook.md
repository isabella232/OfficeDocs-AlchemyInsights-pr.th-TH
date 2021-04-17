---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836154"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ได้

**มีปัญหาที่เจ้าของโฟลเดอร์สาธารณะสร้างโฟลเดอร์ย่อยโดยใช้ Outlook อย่างต่อเนื่อง ปัญหานี้จะได้รับการแก้ไขในเร็วๆ นี้**

ขณะเดียวกัน ให้ใช้วิธีแก้ไขปัญหาชั่วคราวข้อใดข้อหนึ่งต่อไปนี้

1. ใช้ Outlook for MAC เพื่อสร้างโฟลเดอร์ย่อยเนื่องจากปัญหาส่งผลกระทบต่อ Outlook for Windows บนเดสก์ท็อปเท่านั้น (ทุกเวอร์ชัน)
2. ให้ผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ EXO Shell หรือ EAC
3. เปลี่ยน DefaultPublicFolderMailbox/EffectivePublicFolderMailbox บนผู้ใช้เป็นกล่องจดหมายอื่นนอกเหนือจากกล่องจดหมายเนื้อหาของโฟลเดอร์ที่ทําให้เกิดปัญหา  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. รอหนึ่งชั่วโมง รีสตาร์ตไคลเอ็นต์ Outlook