---
title: เลี่ยงผ่านล็อบบี้
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684969"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>ควบคุมการตั้งค่าล็อบบี้และระดับการเข้าร่วมในทีม

ถ้าคุณต้องการอนุญาตให้ทุกคนรวมถึงผู้ใช้การโทรเข้าภายนอกและผู้ใช้ที่ไม่ระบุชื่อเพื่อ **เลี่ยงผ่านล็อบบี้**ให้ใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จ ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Cmdlet นี้จำเป็นต้องใช้โมดูล PowerShell ของ Skype for Business ในขณะนี้ เมื่อต้องการตั้งค่าให้ใช้ cmdlet นี้ให้ดูที่[นโยบายการจัดการผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

เมื่อคุณตั้งค่านโยบายแล้วคุณจำเป็นต้องนำไปใช้กับผู้ใช้ หรือถ้าคุณได้ปรับเปลี่ยนนโยบายส่วนกลางแล้วโปรแกรมจะนำไปใช้กับผู้ใช้โดยอัตโนมัติ สำหรับการเปลี่ยนแปลงนโยบายใดๆคุณจำเป็นต้องรออย่างน้อย **4 ชั่วโมงจนถึง24ชั่วโมง** เพื่อให้นโยบายมีผลบังคับใช้ 

ตรวจสอบให้แน่ใจว่าได้ตรวจสอบเอกสารด้านล่างก่อนที่จะทำการเปลี่ยนแปลงเหล่านี้เพื่อทำความเข้าใจว่าสิ่งนี้จะช่วยได้อย่างไร


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>การทำความเข้าใจเกี่ยวกับการควบคุมนโยบายล็อบบี้การประชุมของทีม

การตั้งค่าเหล่านี้จะควบคุมการประชุมที่ผู้เข้าร่วมประชุมรอในล็อบบี้ก่อนที่พวกเขาจะเข้าร่วมการประชุมและระดับของการเข้าร่วมที่พวกเขาได้รับอนุญาตในการประชุม คุณสามารถใช้ PowerShell เพื่ออัปเดตการตั้งค่านโยบายการประชุมที่ยังไม่ได้นำมาใช้ (ที่มีป้ายชื่อว่า "มาเร็วๆนี้") ในศูนย์การจัดการทีม ให้ดูที่ด้านล่างสำหรับ cmdlet PowerShell ตัวอย่างที่อนุญาตให้ผู้ใช้ทั้งหมดสามารถเลี่ยงผ่านล็อบบี้ได้

- ยอมรับบุคคลที่เป็นนโยบายต่อผู้จัดการ[โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)ที่ควบคุมว่าจะให้ผู้อื่นเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะเข้าร่วมโดยผู้ใช้ที่ได้รับการรับรองความถูกต้อง

- [อนุญาตให้ผู้ใช้ที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้โดยไม่มีผู้ใช้ที่ได้รับการรับรองความถูกต้องจากองค์กรในการเข้าร่วม

- [อนุญาตให้ผู้ใช้ที่โทรเข้าเพื่อเลี่ยงผ่านล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าบุคคลที่โทรเข้าเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**บุคคลที่ยอมรับโดยอัตโนมัติ**

- [อนุญาตให้ผู้จัดที่จะแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ตั้งค่าผู้ดูแลได้ **โดยอัตโนมัติ** และ **อนุญาตให้ผู้ใช้โทรเข้าเพื่อเลี่ยงผ่านล็อบบี้** เมื่อพวกเขาจัดกำหนดการการประชุมใหม่

**หมายเหตุ:** อ่าน [จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) สำหรับภาพรวมที่สมบูรณ์ของนโยบายการประชุมของ Microsoft team
