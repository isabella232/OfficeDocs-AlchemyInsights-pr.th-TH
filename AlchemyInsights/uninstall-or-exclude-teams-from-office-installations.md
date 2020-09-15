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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="2e237-102">ถอนการติดตั้งหรือไม่รวมทีมออกจากการติดตั้งใหม่หรือการติดตั้ง Office ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="2e237-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="2e237-103">ทีม microsoft จะรวมเป็นส่วนหนึ่งของแอป Microsoft ๓๖๕สำหรับองค์กรแอป Microsoft ๓๖๕สำหรับธุรกิจและ Office for Mac</span><span class="sxs-lookup"><span data-stu-id="2e237-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="2e237-104">ใช้ [เครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) เพื่อแยกทีมออกจากการติดตั้ง office ใหม่</span><span class="sxs-lookup"><span data-stu-id="2e237-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="2e237-105">เมื่อต้อง*การถอนการติดตั้ง*ทีมจากอุปกรณ์ที่ใช้ Windows ให้ดูที่[ถอนการติดตั้งทีม Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="2e237-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="2e237-106">เมื่อต้องการล้างข้อมูลทีม Microsoft จากเครื่องจักรเป้าหมายหรือผู้ใช้หลายคนให้ดูที่การล้างข้อมูลการ [ปรับใช้ Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)team</span><span class="sxs-lookup"><span data-stu-id="2e237-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="2e237-107">ใช้ตัวเลือก [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) เพื่อป้องกันไม่ให้ทีม Microsoft ติดตั้งโดยอัตโนมัติด้วย Office</span><span class="sxs-lookup"><span data-stu-id="2e237-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="2e237-108">ใช้ตัวเลือก [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่ทีมจะได้รับการติดตั้ง*เพื่อป้องกันไม่ให้ทีมของ Microsoft เริ่มต้นโดยอัตโนมัติหลังจากการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="2e237-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="2e237-109">ถ้าคุณกำลังใช้ Office for Mac ให้ดูที่[การติดตั้ง Microsoft team บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="2e237-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>