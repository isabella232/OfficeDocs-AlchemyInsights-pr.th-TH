---
title: ถอนการติดตั้งหรือแยก Teams ออกจากการติดตั้ง Office
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
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827811"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>ถอนการติดตั้งหรือแยก Teams จากการติดตั้ง Office ใหม่หรือที่มีอยู่

Microsoft Teams รวมอยู่ใน Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.

- ใช้เครื่องมือ [การปรับใช้ Office เพื่อ](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) แยก Teams จากการติดตั้ง Office ใหม่
- เมื่อต้องการ *ถอนการติดตั้ง* Teams ออกจากอุปกรณ์ที่ใช้ Windows [ให้ดู ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้าง Microsoft Teams จากเครื่องเป้าหมายหรือผู้ใช้หลายราย[ให้ดู การล้างข้อมูลการปรับใช้ Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- ใช้ [ตัวเลือก PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) เพื่อป้องกันไม่ให้ Microsoft Teams ติดตั้งโดยอัตโนมัติกับ Office
- ใช้ [ตัวเลือก PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่จะติดตั้ง Teams* เพื่อป้องกันไม่ให้ Microsoft Teams เริ่มโดยอัตโนมัติหลังจากการติดตั้ง

ถ้าคุณใช้งาน Office for Mac ให้ดู[การติดตั้ง Microsoft Teams บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)