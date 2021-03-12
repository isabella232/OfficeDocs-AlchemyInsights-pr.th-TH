---
title: การตั้งค่านโยบายการประชุม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704625"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมใน Microsoft Teams

**หมายเหตุ: อาจต้องใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลกับผู้ใช้** คุณอาจไม่สามารถเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ 4 ชั่วโมงและพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง

นโยบายการประชุมจะถูกใช้เพื่อควบคุมฟีเจอร์ที่พร้อมใช้งานกับผู้เข้าร่วมการประชุมของการประชุมที่ถูกจัดเวลาโดยผู้ใช้ในองค์กรของคุณ ฟีเจอร์บางอย่างของนโยบายการประชุมอาจยังไม่มีการปรับใช้ในศูนย์การจัดการ Teams (จะมีป้ายชื่อ "เร็วๆ นี้" ในเอกสาร) ในกรณีนี้ หรือถ้าคุณได้รับข้อผิดพลาด เช่น "เราไม่สามารถอัปเดตนโยบายได้ในขณะนี้ แต่ลองอีกครั้งในภายหลัง" ในศูนย์การจัดการ Microsoft Teams เราขอแนะนนะให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุม Teams 

ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมที่แหล่งข้อมูลต่อไปนี้

- เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบาย การเปลี่ยนแปลง และการกําหนดผู้ใช้ให้กับนโยบาย ให้ดูที่[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- เมื่อต้องการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell ให้ดู [ภาพรวม PowerShell ของ](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)Teams 
    - คุณต้องใช้มอดู [ล PowerShell ของ Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) เพื่อใช้งานนโยบายการประชุม Teams 
    - ตรวจทาน [เอกสาร cmdlets *-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) เพื่อดูข้อมูลเพิ่มเติม

