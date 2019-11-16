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
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769826"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="77ff4-102">ถอนการติดตั้งหรือยกเว้นทีมจากการติดตั้ง Office ใหม่หรือที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="77ff4-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="77ff4-103">Microsoft Teams จะรวมเป็นส่วนหนึ่งของ Office ๓๖๕ ProPlus, Office ๓๖๕ธุรกิจและ Office สำหรับ Mac</span><span class="sxs-lookup"><span data-stu-id="77ff4-103">Microsoft Teams is included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="77ff4-104">ใช้[เครื่องมือการปรับใช้ office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)เพื่อยกเว้นทีมจากการติดตั้ง Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="77ff4-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="77ff4-105">ในการ*ถอนการติดตั้ง*ทีมจากอุปกรณ์ที่ใช้ Windows โปรดดูที่[ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="77ff4-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="77ff4-106">หากต้องการล้างข้อมูลทีม Microsoft จากเครื่องหลายเป้าหมายหรือผู้ใช้ให้ดูที่[Microsoft teams ปรับใช้การล้างข้อมูล](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="77ff4-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="77ff4-107">ใช้ตัวเลือกการป้องกัน[Teamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)เพื่อไม่ให้ Microsoft Teams ติดตั้งโดยอัตโนมัติกับ Office</span><span class="sxs-lookup"><span data-stu-id="77ff4-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="77ff4-108">ใช้ตัวเลือก[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่ทีมจะถูกติดตั้ง*เพื่อป้องกันไม่ให้ Microsoft Teams เริ่มต้นโดยอัตโนมัติหลังจากการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="77ff4-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="77ff4-109">ถ้าคุณกำลังใช้ Office สำหรับ Mac โปรดดูที่[การติดตั้ง Microsoft Teams บน mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="77ff4-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>