---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063143"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้Outlook

**มีปัญหาที่เจ้าของโฟลเดอร์สาธารณะสร้างโฟลเดอร์ย่อยโดยใช้โฟลเดอร์Outlookอยู่ ปัญหานี้จะได้รับการแก้ไขในเร็วๆ นี้**

ขณะเดียวกัน ให้ใช้วิธีแก้ไขปัญหาชั่วคราวข้อใดข้อหนึ่งต่อไปนี้

1. ใช้ Outlook for MAC เพื่อสร้างโฟลเดอร์ย่อยเนื่องจากปัญหาส่งผลกระทบเฉพาะOutlook Windows บนเดสก์ท็อป (ทุกเวอร์ชัน)
2. ให้ผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ EXO Shell หรือ EAC
3. เปลี่ยน DefaultPublicFolderMailbox/EffectivePublicFolderMailbox บนผู้ใช้เป็นกล่องจดหมายอื่นนอกเหนือจากกล่องจดหมายเนื้อหาของโฟลเดอร์ที่ทําให้เกิดปัญหา  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. รอหนึ่งชั่วโมง รีสตาร์ตไคลเอ็นต์ Outlook