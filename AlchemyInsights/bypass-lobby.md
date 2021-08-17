---
title: การเลี่ยงผ่านล็อบบี้
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
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059615"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>ควบคุมการตั้งค่าล็อบบี้และระดับของการมีส่วนร่วมในTeams

ถ้าคุณต้องการอนุญาตให้ทุกคน รวมถึง Dial-in, ผู้ใช้ภายนอก และผู้ใช้ที่ไม่ระบุชื่อ สามารถเลี่ยงผ่านล็อบบี้ ได้ ให้ใช้ PowerShell เพื่อทํางานนี้ให้เสร็จสมบูรณ์ ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางขององค์กรของคุณ

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

cmdlet นี้ต้องใช้โมดูล powershell Skype for Businessในขณะนี้ เมื่อต้องการตั้งค่าเพื่อใช้ cmdlet นี้ ให้ตรวจสอบ[การจัดการนโยบายผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

เมื่อคุณตั้งค่านโยบายแล้ว คุณจึงต้องปรับใช้นโยบายกับผู้ใช้ หรือหากคุณปรับเปลี่ยนนโยบายส่วนกลาง นโยบายจะมีผลบังคับใช้กับผู้ใช้โดยอัตโนมัติ เพื่อให้การเปลี่ยนแปลงนโยบายมีผล อย่างน้อย **4 ชั่วโมงจึงจะถึง 24** ชั่วโมงเพื่อให้นโยบายมีผล 

อย่าลืมตรวจทานเอกสารประกอบด้านล่างก่อนการเปลี่ยนแปลงเหล่านี้เพื่อเข้าใจว่าสิ่งนี้อนุญาตคืออะไร


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>การTeamsตัวควบคุมนโยบายล็อบบี้การประชุม

การตั้งค่าเหล่านี้จะควบคุมว่าผู้เข้าร่วมการประชุมคนใดจะต้องรอในล็อบบี้ก่อนได้รับการยอมรับให้เข้าร่วมการประชุมและระดับการมีส่วนร่วมในการประชุม คุณสามารถใช้ PowerShell เพื่ออัปเดตการตั้งค่านโยบายการประชุมที่ยังไม่ได้ปรับใช้ (ที่มีป้ายชื่อ "เร็วๆ นี้") ในศูนย์Teamsการประชุม See below for an example PowerShell cmdlet that allows all users to bypass the lobby.

- [ยอมรับบุคคลโดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) เป็นนโยบายต่อผู้จัดที่จะควบคุมว่าบุคคลที่เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าได้รับการยอมรับจากผู้ใช้ที่ได้รับการรับรองความถูกต้อง

- [Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federrated users, can join the user's meeting without an authenticated user from the organization in attendance.

- [อนุญาตให้ผู้ใช้โทร](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)เข้าเพื่อข้ามล็อบบี้ **(เร็ว** ๆ นี้ ) เป็นนโยบายต่อผู้จัดการประชุมที่ควบคุมว่าบุคคลที่โทรเข้าทางโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่เกี่ยวกับการตั้งค่า ยอมรับ **บุคคลโดยอัตโนมัติ**

- [อนุญาตให้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)ผู้จัดการประชุมแทนที่การตั้งค่าล็อบบี้ **(เร็ว** ๆ นี้ ) เป็นนโยบายต่อผู้จัดการประชุมที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลระบบตั้งค่าในยอมรับบุคคลและอนุญาตให้ผู้ใช้โทรเข้าโดยอัตโนมัติ หรือไม่เพื่อเลี่ยงผ่านล็อบบี้เมื่อพวกเขาจัดเวลาการประชุมใหม่

**หมายเหตุ:** อ่าน [จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมโดยสมบูรณ์ของMicrosoft Teamsนโยบายการประชุม
