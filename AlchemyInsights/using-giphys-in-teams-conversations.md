---
title: การใช้ Giphys ในการสนทนาของทีม
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982575"
---
# <a name="using-giphys-in-teams-conversations"></a>การใช้ Giphys ในการสนทนาของทีม

การเข้าถึง Giphys ในทีมการสนทนาจะถูกเปิดใช้งานตามค่าเริ่มต้น **ใน** ฐานะผู้ดูแลระบบคุณสามารถควบคุมได้ว่า Giphys จะพร้อมใช้งานสำหรับผู้ใช้โดย [การตั้งค่านโยบายการส่งข้อความ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)และตรวจสอบให้แน่ใจว่า **ใช้ Giphys ในการสนทนา**

ถ้า GIFs ไม่ทำงานตามที่คาดไว้ในการสนทนาของทีมให้ตรวจสอบดังนี้

[นโยบายการส่งข้อ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)ความจำเป็นต้องมีการอนุญาตให้ Giphys เมื่อต้องการตรวจสอบโดยใช้ cmdlet ของ PowerShell ให้ใช้วิธีต่อไปนี้

- ตรวจสอบว่าคุณสามารถ [จัดการทีมด้วย PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)ได้
- เรียกใช้คำสั่ง PowerShell [ได้รับ-CsTeamsMessagingPolicy-ข้อมูลประจำตัว-ส่วนกลาง](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps)และตรวจสอบว่า **AllowGiphy** ถูกตั้งค่าเป็น **TRUE**
- ถ้า **AllowGiphy** ถูกตั้งค่าเป็น **FALSE** ให้เรียกใช้คำสั่ง PowerShell ชุดต่อไปนี้ [-CsTeamsMessagingPolicy-ข้อมูลประจำตัว AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

จำเป็นต้องเปิดใช้งานการ[เชื่อมต่อ](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)ที่ไม่จำเป็นต้องเปิดใช้งานเพื่ออนุญาตการเข้าถึง URL Giphy

> [!NOTE]
> ถ้าคุณมีนโยบายการส่งข้อความหลายทีมที่กำหนดค่าสำหรับผู้เช่าของคุณคุณสามารถกำหนดข้อมูลเฉพาะตัวของนโยบายที่กำหนดให้กับผู้ใช้ที่ได้รับผลกระทบที่มีคำสั่ง PowerShell ที่ [ได้รับการ CsOnlineUser-ข้อมูลประจำตัว](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> เลือก TeamsMessagingPolicy
