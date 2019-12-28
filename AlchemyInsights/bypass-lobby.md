---
title: ล็อบบี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889101"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>ควบคุมการตั้งค่าล็อบบี้และระดับการเข้าร่วมทีม

หากคุณต้องการอนุญาตให้ทุกคนรวมถึงการเรียกเลขหมายภายนอกและผู้ใช้ที่ไม่ระบุชื่อให้**ข้ามล็อบบี้**ให้ใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จ ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet นี้จำเป็นต้องใช้ Skype สำหรับโมดูล PowerShell ธุรกิจในขณะนี้ หากต้องการรับการตั้งค่าเพื่อใช้ cmdlet นี้ให้ตรวจสอบ[นโยบายการจัดการผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

เมื่อคุณตั้งค่านโยบายแล้วคุณจะต้องนำไปใช้กับผู้ใช้ หรือถ้าคุณปรับเปลี่ยนนโยบายสากลระบบจะนำไปใช้กับผู้ใช้โดยอัตโนมัติ สำหรับการเปลี่ยนแปลงนโยบายใดๆคุณต้องรออย่างน้อย**4 ชั่วโมงจนถึง24ชั่วโมง**เพื่อให้นโยบายมีผลบังคับใช้ 

ตรวจสอบให้แน่ใจว่าได้ตรวจสอบเอกสารด้านล่างก่อนที่จะทำการเปลี่ยนแปลงเหล่านี้เพื่อให้เข้าใจว่าสิ่งนี้ช่วยได้อย่างไร


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>ทำความเข้าใจเกี่ยวกับการควบคุมทีมงานการประชุมนโยบายล็อบบี้

การตั้งค่าเหล่านี้จะควบคุมผู้เข้าร่วมประชุมที่รออยู่ในล็อบบี้ก่อนที่จะเข้ารับการประชุมและระดับการเข้าร่วมประชุมที่ได้รับอนุญาต คุณสามารถใช้ PowerShell เพื่อปรับปรุงการตั้งค่านโยบายการประชุมที่ยังไม่ได้ดำเนินการ (ที่มีป้ายชื่อ "เร็วๆนี้") ในศูนย์การจัดการทีม ดูด้านล่างสำหรับตัวอย่าง cmdlet PowerShell ที่ช่วยให้ผู้ใช้ทั้งหมดที่จะข้ามล็อบบี้

- [ยอมรับผู้ใช้โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้คนเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะได้รับการตรวจสอบโดยผู้ที่รับรองความถูกต้อง

- [อนุญาตให้บุคคลที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้แบบ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้ได้โดยไม่มีผู้ใช้ที่รับรองความถูกต้องจากองค์กรในการเข้างาน

- [อนุญาตให้ผู้ใช้โทรออกในการข้ามล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้ที่เรียกเลขหมายโดยโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**ผู้คนที่ยอมรับโดยอัตโนมัติ**

- [อนุญาตให้ผู้จัดทำการแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)(**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดการที่ควบคุมว่าการประชุมผู้จัดการสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลระบบตั้งค่าไว้**โดยอัตโนมัติยอมรับบุคคล**และ**อนุญาตให้ใช้การเรียกเลขหมายในการข้ามล็อบบี้**เมื่อพวกเขาจัดตารางเวลาการประชุมใหม่

**หมายเหตุ:** อ่าน[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมทั้งหมดของนโยบายการประชุมของ Microsoft Teams
