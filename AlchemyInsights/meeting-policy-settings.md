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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042863"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมในทีมของ Microsoft

**หมายเหตุ: อาจใช้เวลาถึง24ชั่วโมงสำหรับการเปลี่ยนแปลงนโยบายที่จะมีผลสำหรับผู้ใช้** คุณอาจไม่สามารถทำการเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามที่จะปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง

นโยบายการประชุมจะใช้ในการควบคุมลักษณะการทำงานที่มีให้กับผู้เข้าร่วมประชุมสำหรับการประชุมที่ได้รับการจัดกำหนดการไว้ในองค์กรของคุณ คุณลักษณะบางอย่างของนโยบายการประชุมอาจไม่ได้ถูกนำมาใช้ในศูนย์การจัดการทีมยัง (เหล่านี้จะมีป้ายชื่อว่า "เร็วๆนี้" ในเอกสารประกอบ) ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถปรับปรุงนโยบายในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์ผู้ดูแลของ Microsoft ทีมเราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมดูทรัพยากรต่อไปนี้:

- เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายให้ทำการเปลี่ยนแปลงและกำหนดผู้ใช้ให้กับนโยบายโปรดดู[ที่จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- เมื่อต้องการทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlets PowerShell ให้ดูที่[ภาพรวมของทีม PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณจำเป็นต้องใช้[Skype สำหรับโมดูล PowerShell ธุรกิจ](https://www.microsoft.com/download/details.aspx?id=39366)สำหรับทีมนโยบายการประชุม 
    - ตรวจทานการ[*-CsTeamsMeetingPolicy cmdlet ของเอกสาร](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)สำหรับข้อมูลเพิ่มเติม

