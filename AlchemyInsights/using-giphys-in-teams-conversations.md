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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104327"
---
# <a name="using-giphys-in-teams-conversations"></a>การใช้ Giphys Teamsการสนทนา

การเข้าถึง Giphys Teamsการแชทของคุณจะถูกเปิดใช้งานตามค่าเริ่มต้น ในฐานะผู้ดูแลระบบ คุณสามารถควบคุมได้ถ้า Giphys พร้อมใช้งานกับผู้ใช้โดยการตั้งค่า [นโยบาย](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) การส่งข้อความ และตรวจสอบว่า **ใช้ Giphys ใน** การสนทนา **เป็น** เปิด

หาก GIF ไม่ใช้งานได้ตามที่คาดไว้ในTeams ให้ตรวจสอบว่า:

นโยบาย [การส่งข้อความ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ต้องอนุญาต Giphys เมื่อต้องการตรวจสอบโดยใช้ PowerShell cmdlets:

- ตรวจสอบว่าคุณสามารถ จัดการ[Teams ด้วย PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- เรียกใช้สั่ง PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps)และตรวจสอบว่า **AllowGiphy** ถูกตั้งค่า **เป็น TRUE**
- ถ้า **AllowGiphy** ถูกตั้งค่าเป็น **FALSE** ให้เรียกใช้การสั่ง PowerShell ต่อไปนี้ [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[ประสบการณ์การเชื่อมต่อเสริม](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) ต้องเปิดใช้งานเพื่ออนุญาตให้เข้าถึง URL Giphy

> [!NOTE]
> If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | เลือก TeamsMessagingPolicy
