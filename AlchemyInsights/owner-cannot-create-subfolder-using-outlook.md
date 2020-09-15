---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665737"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook

**มีปัญหาที่เกิดขึ้นอย่างต่อเนื่องกับเจ้าของโฟลเดอร์สาธารณะการสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ปัญหานี้จะได้รับการแก้ไขในเร็วๆนี้**

ในขณะเดียวกันให้ใช้หนึ่งในวิธีการแก้ไขปัญหาต่อไปนี้:

1. ใช้ Outlook for MAC เพื่อสร้างโฟลเดอร์ย่อยเป็นปัญหาที่มีผลต่อ Outlook สำหรับเดสก์ท็อป windows (ทุกเวอร์ชัน)
2. มีผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ Shell หรือ EAC
3. เปลี่ยน DefaultPublicFolderMailbox/EffectivePublicFolderMailbox บนผู้ใช้ไปยังกล่องจดหมายอื่นที่ไม่ใช่กล่องจดหมายเนื้อหาสำหรับโฟลเดอร์ที่ทำให้เกิดปัญหา  
    - *ตั้งค่ากล่องจดหมาย User1 DefaultPublicFolderMailbox PubMBX3*
4. รอสักครู่ให้เริ่มไคลเอ็นต์ outlook ใหม่