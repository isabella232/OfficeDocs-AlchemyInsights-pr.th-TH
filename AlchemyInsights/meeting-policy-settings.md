---
title: การตั้งค่านโยบายการประชุม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627593"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมใน Microsoft Teams

นโยบายการประชุมจะใช้ในการควบคุมคุณลักษณะที่พร้อมใช้งานสำหรับผู้เข้าร่วมประชุมสำหรับการประชุมที่มีการจัดตารางการผลิตระดับผู้ใช้ในองค์กรของคุณ คุณลักษณะบางอย่างของนโยบายการประชุมอาจไม่ได้ดำเนินการในศูนย์กลางการดูแลระบบ (ซึ่งมีป้ายชื่อ "เร็วๆนี้" ในเอกสารประกอบ) ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถปรับปรุงนโยบายในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์กลางการดูแล Microsoft Teams เราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมโปรดดูทรัพยากรต่อไปนี้:

- หากต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายทำการเปลี่ยนแปลงและกำหนดผู้ใช้ให้กับนโยบายโปรดดูที่[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- เพื่อทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet[ของ powershell ดูภาพรวมของทีม powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณจำเป็นต้องใช้[Skype สำหรับโมดูล PowerShell ธุรกิจ](https://www.microsoft.com/download/details.aspx?id=39366)สำหรับนโยบายการประชุมทีม 
    - ตรวจทาน[เอกสารการ cmdlet ของ *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)สำหรับข้อมูลเพิ่มเติม

**หมายเหตุ:** การเปลี่ยนแปลงนโยบายอาจใช้เวลาถึง24ชั่วโมงจึงจะมีผลสำหรับผู้ใช้ คุณอาจไม่สามารถทำการเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามที่จะปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง หากคุณยังคงมีปัญหาอยู่ให้ลองใช้ PowerShell  