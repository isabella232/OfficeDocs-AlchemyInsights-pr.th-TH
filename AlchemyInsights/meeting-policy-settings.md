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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794353"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>จัดการนโยบายการประชุมในทีม Microsoft

**หมายเหตุ: อาจใช้เวลาถึง24ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลต่อผู้ใช้** คุณอาจไม่สามารถทำการเปลี่ยนแปลงไปยังนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง

นโยบายการประชุมจะถูกใช้ในการควบคุมฟีเจอร์ที่พร้อมใช้งานสำหรับผู้เข้าร่วมการประชุมสำหรับการประชุมที่จัดกำหนดการโดยผู้ใช้ในองค์กรของคุณ ฟีเจอร์บางอย่างของนโยบายการประชุมอาจไม่ถูกนำไปใช้ในศูนย์การจัดการทีมยัง (เหล่านี้จะมีป้ายชื่อว่า "มาเร็วๆนี้" ในเอกสารประกอบ) ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถอัปเดตรายละเอียดได้ในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์การจัดการทีมของ Microsoft เราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมให้ดูที่แหล่งข้อมูลต่อไปนี้:

- เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายการทำการเปลี่ยนแปลงและการกำหนดผู้ใช้ให้กับนโยบายให้ดูที่[จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- เมื่อต้องการทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell ให้ดูที่[ภาพรวมของทีม PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - คุณจำเป็นต้องใช้ [โมดูล PowerShell ของ Skype For business](https://www.microsoft.com/download/details.aspx?id=39366) สำหรับนโยบายการประชุมของทีม 
    - ตรวจทาน [คู่มือ cmdlet ของ CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) สำหรับข้อมูลเพิ่มเติม

