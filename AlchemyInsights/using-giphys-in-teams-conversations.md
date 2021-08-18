---
title: การใช้ Giphys Teamsการสนทนา
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323539"
---
# <a name="using-giphys-in-teams-conversations"></a>การใช้ Giphys Teamsการสนทนา

การเข้าถึง Giphys Teamsการแชทของคุณจะถูกเปิดใช้งานตามค่าเริ่มต้น ในฐานะผู้ดูแลระบบ คุณสามารถควบคุมได้ถ้า Giphys พร้อมใช้งานกับผู้ใช้ โดยการตั้งค่า [นโยบาย](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) การส่งข้อความ และตรวจสอบว่า **ใช้ Giphys ใน** การสนทนา **เป็น** เปิด

หาก GIF ไม่เป็นไปตามที่คาดไว้ในTeams ให้ตรวจสอบว่า:

นโยบาย [การส่งข้อความ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ต้องอนุญาต Giphys เมื่อต้องการตรวจสอบโดยใช้ PowerShell cmdlets:

- ตรวจสอบว่า คุณสามารถ จัดการ[Teams ด้วย PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- เรียกใช้สั่ง PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps)และตรวจสอบว่า **AllowGiphy** ถูกตั้งค่า **เป็น TRUE**
- ถ้า **AllowGiphy** ถูกตั้งค่า **เป็น FALSE** ให้เรียกใช้การสั่ง PowerShell ต่อไปนี้ [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[ประสบการณ์การเชื่อมต่อเสริม](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) ต้องเปิดใช้งานเพื่ออนุญาตให้เข้าถึง URL Giphy

**หมายเหตุ**: ถ้าคุณกําหนดค่านโยบายการส่งข้อความ Teams หลายนโยบายให้กับผู้เช่าของคุณ คุณสามารถกําหนดข้อมูลเฉพาะตัวของนโยบายที่กําหนดให้กับผู้ใช้ได้รับผลกระทบด้วยสั่ง PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | เลือก TeamsMessagingPolicy
