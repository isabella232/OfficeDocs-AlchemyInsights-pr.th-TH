---
title: ถอนการติดตั้งหรือแยกทีมออกจากการติดตั้ง Office
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
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010336"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="be27d-102">ถอนการติดตั้งหรือแยกทีมออกจากการติดตั้ง Office ใหม่หรือที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="be27d-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="be27d-103">Microsoft Teams จะรวมเป็นส่วนหนึ่งของแอป Microsoft 365 สําหรับธุรกิจ, Microsoft 365 Apps สําหรับธุรกิจ และ Office for Mac</span><span class="sxs-lookup"><span data-stu-id="be27d-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="be27d-104">ใช้เครื่องมือ[การปรับใช้ Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)เพื่อแยกทีมจากการติดตั้งใหม่ของ Office</span><span class="sxs-lookup"><span data-stu-id="be27d-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="be27d-105">เมื่อต้องการ*ถอนการติดตั้ง*ทีมจากอุปกรณ์ที่เรียกใช้ Windows ให้ดูที่[การถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="be27d-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="be27d-106">เมื่อต้องการล้างข้อมูล Microsoft Teams จากเครื่องเป้าหมายหรือผู้ใช้หลายราย ให้ดูที่[การปรับใช้ Microsoft Teams ล้างข้อมูล](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="be27d-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="be27d-107">ใช้ตัวเลือก[ป้องกัน TeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)เพื่อป้องกันไม่ให้ทีม Microsoft ติดตั้งโดยอัตโนมัติด้วย Office</span><span class="sxs-lookup"><span data-stu-id="be27d-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="be27d-108">ใช้ตัวเลือก[ป้องกันFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่ Teams จะถูกติดตั้ง*เพื่อป้องกันไม่ให้ทีม Microsoft เริ่มทํางานโดยอัตโนมัติหลังจากการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="be27d-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="be27d-109">ถ้าคุณกําลังใช้ Office สําหรับ Mac ให้ดูที่[การติดตั้ง Microsoft Teams บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="be27d-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>