---
title: ถอนการติดตั้งหรือไม่รวมTeamsการติดตั้งOfficeออก
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007737"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>ถอนการติดตั้งหรือTeamsการติดตั้งใหม่หรือOfficeที่มีอยู่

Microsoft Teamsจะถูกรวมเป็นส่วนหนึ่งของMicrosoft 365 Apps for enterprise Microsoft 365 Apps for business และOffice for Mac

- ใช้เครื่องมือ[Officeการปรับใช้เพื่อ](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)Teamsออกจากการติดตั้งใหม่Office
- เมื่อต้องการ *Teams* ออกจากอุปกรณ์Windowsอุปกรณ์ของคุณ ให้ดู [ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- ใช้[ตัวเลือก PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)เพื่อMicrosoft Teamsไม่ให้ติดตั้งโดยอัตโนมัติOfficeการติดตั้ง
- ใช้ [ตัวเลือก PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่จะTeamsติดตั้ง* ใหม่ เพื่อป้องกันไม่ให้ Microsoft Teams เริ่มโดยอัตโนมัติหลังจากการติดตั้ง

หากคุณใช้งาน Office for Mac โปรดดู[Microsoft Teamsบน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)