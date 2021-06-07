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
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794144"
---
# <a name="manage-webinar-registration"></a>จัดการการลงทะเบียนการสัมมนาผ่านเว็บ

คุณสามารถจัดการผู้ที่สามารถลงทะเบียนเข้าร่วมTeamsสัมมนาผ่านเว็บโดยใช้Teamsสั่ง Powershell เมื่อต้องการTeams Powershell [Teams PowerShell](/microsoftteams/teams-powershell-install) 

ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและตั้งค่า **เป็น EveryoneInCompany** To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**หมายเหตุ**: ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้ เมื่อต้องการเรียนรู้เพิ่มเติมและเปิดใช้งานการตั้งค่านี้[ให้ดู จัดการการตั้งค่าการประชุมใน Microsoft Teams](/microsoftteams/meeting-settings-in-teams)

ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).
