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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376873"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>ควบคุมการตั้งค่าและระดับการเข้าร่วมของล็อบบี้

การตั้งค่าเหล่านี้จะควบคุมผู้เข้าร่วมประชุมที่รออยู่ในล็อบบี้ก่อนที่จะเข้ารับการประชุมและระดับการเข้าร่วมประชุมที่ได้รับอนุญาต คุณสามารถใช้ Powershell เพื่อปรับปรุงการตั้งค่านโยบายการประชุมที่ยังไม่ได้ดำเนินการ (ที่มีป้ายชื่อ "เร็วๆนี้") ในศูนย์การจัดการทีม  ดูด้านล่างสำหรับตัวอย่าง cmdlet PowerShell ที่ช่วยให้ผู้ใช้ทั้งหมดที่จะข้ามล็อบบี้  

- [ยอมรับผู้ใช้โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้คนเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะได้รับการตรวจสอบโดยผู้ที่รับรองความถูกต้อง

- [อนุญาตให้บุคคลที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้แบบ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้ได้โดยไม่มีผู้ใช้ที่รับรองความถูกต้องจากองค์กรในการเข้างาน

- [อนุญาตให้ผู้ใช้โทรออกในการข้ามล็อบบี้](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้ที่เรียกเลขหมายโดยโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**ผู้คนที่ยอมรับโดยอัตโนมัติ**

- [อนุญาตให้ผู้จัดการแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลตั้งค่า**โดยอัตโนมัติยอมรับคน**และ**อนุญาตให้มีการเรียกเลขหมาย ผู้ใช้ที่จะข้ามล็อบบี้**เมื่อพวกเขาจัดกำหนดการการประชุมใหม่

**หมายเหตุ:** อ่าน[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมทั้งหมดของนโยบายการประชุมของ Microsoft Teams 


**ตัวอย่างของ PowerShell**

หากคุณต้องการอนุญาตให้ทุกคนรวมถึงผู้ใช้ภายนอกหรือไม่ระบุชื่อให้ข้ามล็อบบี้คุณยังสามารถใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จได้  ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ   

(โปรดตรวจสอบเอกสารดังกล่าวข้างต้นก่อนทำการเปลี่ยนแปลงเหล่านี้เพื่อให้เข้าใจว่าสิ่งนี้ช่วยได้อย่างไร)

ชุด-CsTeamsMeetingPolicy-อัตลักษณ์ทั่วโลก-AutoAdmittedUsers "ทุกคน"-AllowPSTNUsersToBypassLobby $True

สำหรับข้อมูลเพิ่มเติมโปรดดูที่[ชุด-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)
