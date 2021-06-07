---
title: จัดการการลงทะเบียนการสัมมนาผ่านเว็บ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798663"
---
# <a name="manage-webinar-registration"></a>จัดการการลงทะเบียนการสัมมนาผ่านเว็บ

คุณสามารถจัดการผู้ที่สามารถลงทะเบียนเข้าร่วมTeamsสัมมนาผ่านเว็บโดยใช้Teamsสั่ง Powershell เมื่อต้องการTeams Powershell [Teams PowerShell](/microsoftteams/teams-powershell-install) 

ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและ **ตั้งค่าเป็น** ทุกคน 

ถ้าคุณไม่เห็นตัวเลือกเพื่ออนุญาตการลงทะเบียนให้ทุกคนในคําเชิญเข้าร่วมประชุม ให้เรียกใช้การตั้งค่า *WhoCanRegister ใหม่* เป็น ทุกคน และรอ 24 ชั่วโมง เมื่อต้องการเรียกใช้ *WhoCanRegister ใหม่* ให้ใช้สั่ง Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**หมายเหตุ**: ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้ เมื่อต้องการเรียนรู้เพิ่มเติมและเปิดใช้งานการตั้งค่านี้[ให้ดู จัดการการตั้งค่าการประชุมใน Microsoft Teams](/microsoftteams/meeting-settings-in-teams)

ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).
