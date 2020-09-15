---
title: ถอนการติดตั้งหรือไม่รวมทีมออกจากการติดตั้ง Office
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658240"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>ถอนการติดตั้งหรือไม่รวมทีมออกจากการติดตั้งใหม่หรือการติดตั้ง Office ที่มีอยู่

ทีม microsoft จะรวมเป็นส่วนหนึ่งของแอป Microsoft ๓๖๕สำหรับองค์กรแอป Microsoft ๓๖๕สำหรับธุรกิจและ Office for Mac

- ใช้ [เครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) เพื่อแยกทีมออกจากการติดตั้ง office ใหม่
- เมื่อต้อง*การถอนการติดตั้ง*ทีมจากอุปกรณ์ที่ใช้ Windows ให้ดูที่[ถอนการติดตั้งทีม Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้างข้อมูลทีม Microsoft จากเครื่องจักรเป้าหมายหรือผู้ใช้หลายคนให้ดูที่การล้างข้อมูลการ [ปรับใช้ Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)team
- ใช้ตัวเลือก [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) เพื่อป้องกันไม่ให้ทีม Microsoft ติดตั้งโดยอัตโนมัติด้วย Office
- ใช้ตัวเลือก [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่ทีมจะได้รับการติดตั้ง*เพื่อป้องกันไม่ให้ทีมของ Microsoft เริ่มต้นโดยอัตโนมัติหลังจากการติดตั้ง

ถ้าคุณกำลังใช้ Office for Mac ให้ดูที่[การติดตั้ง Microsoft team บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)