---
title: ถอนการติดตั้งหรือยกเว้นทีมจากการติดตั้ง Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344256"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>ถอนการติดตั้งหรือยกเว้นทีมจากการติดตั้ง Office ใหม่หรือที่มีอยู่

ตอนนี้ทีม Microsoft จะรวมเป็นส่วนหนึ่งของ Office ๓๖๕ ProPlus, Office ๓๖๕ธุรกิจและ Office สำหรับ Mac

- ใช้[เครื่องมือการปรับใช้ office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)เพื่อยกเว้นทีมจากการติดตั้ง Office ใหม่
- ในการ*ถอนการติดตั้ง*ทีมจากอุปกรณ์ที่ใช้ Windows โปรดดูที่[ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) หากต้องการล้างข้อมูลทีม Microsoft จากเครื่องหลายเป้าหมายหรือผู้ใช้ให้ดูที่[Microsoft teams ปรับใช้การล้างข้อมูล](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- ใช้ตัวเลือกการป้องกัน[Teamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)เพื่อไม่ให้ Microsoft Teams ติดตั้งโดยอัตโนมัติกับ Office
- ใช้ตัวเลือก[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่ทีมจะถูกติดตั้ง*เพื่อป้องกันไม่ให้ Microsoft Teams เริ่มต้นโดยอัตโนมัติหลังจากการติดตั้ง

ถ้าคุณกำลังใช้ Office สำหรับ Mac โปรดดูที่[การติดตั้ง Microsoft Teams บน mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)