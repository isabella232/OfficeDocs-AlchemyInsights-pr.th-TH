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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925184"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมใน Microsoft Teams

**หมายเหตุ: อาจต้องใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลกับผู้ใช้** คุณอาจไม่สามารถเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ 4 ชั่วโมง และพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง

นโยบายการประชุมจะถูกใช้เพื่อควบคุมฟีเจอร์ต่างๆ ที่พร้อมใช้งานกับผู้เข้าร่วมประชุมของการประชุมที่จัดเวลาโดยผู้ใช้ในองค์กรของคุณ ฟีเจอร์บางอย่างของนโยบายการประชุมอาจไม่ถูกปรับใช้ในศูนย์การจัดการ Teams (จะมีป้ายชื่อ "เร็วๆ นี้" ในเอกสาร) ในกรณีนี้ หรือถ้าคุณได้รับข้อผิดพลาด เช่น "เราไม่สามารถอัปเดตนโยบายได้ในขณะนี้ แต่ให้ลองอีกครั้งในภายหลัง" ในศูนย์การจัดการ Microsoft Teams เราขอแนะนนะให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุม Teams 

ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมที่แหล่งข้อมูลต่อไปนี้

- เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบาย การเปลี่ยนแปลง และการกําหนดผู้ใช้ให้กับนโยบาย ให้ดูที่ จัดการ[นโยบายการประชุมใน](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)Teams

- เมื่อต้องการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell [Teams ภาพรวม PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณต้องใช้มอดู[ล Skype for Business PowerShell ของคุณ](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)Teamsนโยบายการประชุม 
    - ตรวจทาน [เอกสาร cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) เพื่อดูข้อมูลเพิ่มเติม

