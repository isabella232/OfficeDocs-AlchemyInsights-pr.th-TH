---
title: การตั้งค่านโยบายการประชุม
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825462"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมใน Microsoft Teams

**หมายเหตุ: อาจต้องใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลกับผู้ใช้** คุณอาจไม่สามารถเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ 4 ชั่วโมง และพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง

นโยบายการประชุมจะถูกใช้เพื่อควบคุมฟีเจอร์ต่างๆ ที่พร้อมใช้งานกับผู้เข้าร่วมประชุมของการประชุมที่จัดเวลาโดยผู้ใช้ในองค์กรของคุณ ฟีเจอร์บางอย่างของนโยบายการประชุมอาจไม่ถูกปรับใช้ในศูนย์การจัดการ Teams (มีป้ายชื่อ "เร็วๆ นี้" ในเอกสารประกอบ) ในกรณีนี้ หรือถ้าคุณได้รับข้อผิดพลาด เช่น "เราไม่สามารถอัปเดตนโยบายได้ในขณะนี้ แต่โปรดลองอีกครั้งในภายหลัง" ในศูนย์การจัดการ Microsoft Teams เราขอแนะนนะให้คุณใช้ PowerShell ในการสร้างหรือปรับเปลี่ยนนโยบายการประชุม Teams 

ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมที่แหล่งข้อมูลต่อไปนี้

- เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบาย การเปลี่ยนแปลง และการกําหนดนโยบายให้กับผู้ใช้ ให้ดู[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- เมื่อต้องการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell ให้ดู[ภาพรวมของ Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณต้องใช้มอดู [ล PowerShell ของ Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams นโยบายการประชุม 
    - ตรวจทาน [เอกสาร cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) เพื่อดูข้อมูลเพิ่มเติม

