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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376868"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมใน Microsoft Teams

นโยบายการประชุมจะใช้ในการควบคุมคุณลักษณะที่พร้อมใช้งานสำหรับผู้เข้าร่วมประชุมสำหรับการประชุมที่มีการจัดตารางการผลิตระดับผู้ใช้ในองค์กรของคุณ คุณลักษณะบางอย่างของนโยบายการประชุมอาจไม่ได้ดำเนินการในศูนย์กลางการดูแลระบบ (ซึ่งมีป้ายชื่อ "เร็วๆนี้" ในเอกสารประกอบ) ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถปรับปรุงนโยบายในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์กลางการดูแล Microsoft Teams เราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมโปรดดูทรัพยากรต่อไปนี้:

- หากต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายทำการเปลี่ยนแปลงและกำหนดผู้ใช้ให้กับนโยบายโปรดดูที่[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)

- เพื่อทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet[ของ powershell ดูภาพรวมของทีม powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณจำเป็นต้องใช้[Skype สำหรับโมดูล PowerShell ธุรกิจ](https://www.microsoft.com/download/details.aspx?id=39366)สำหรับนโยบายการประชุมทีม 
    - ตรวจทาน[เอกสารการ cmdlet ของ *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)สำหรับข้อมูลเพิ่มเติม

**หมายเหตุ:** การเปลี่ยนแปลงนโยบายอาจใช้เวลาถึง24ชั่วโมงจึงจะมีผลสำหรับผู้ใช้ คุณอาจไม่สามารถทำการเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามที่จะปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง หากคุณยังคงมีปัญหาอยู่ให้ลองใช้ PowerShell  