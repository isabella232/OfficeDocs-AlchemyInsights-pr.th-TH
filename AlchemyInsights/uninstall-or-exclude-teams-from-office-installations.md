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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="ad08e-102">ถอนการติดตั้งหรือแยก Teams จากการติดตั้ง Office ใหม่หรือที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="ad08e-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="ad08e-103">Microsoft Teams รวมอยู่ใน Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="ad08e-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="ad08e-104">ใช้เครื่องมือ [การปรับใช้ Office เพื่อ](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) แยก Teams จากการติดตั้ง Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="ad08e-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="ad08e-105">เมื่อต้องการ *ถอนการติดตั้ง* Teams ออกจากอุปกรณ์ที่ใช้ Windows [ให้ดู ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="ad08e-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="ad08e-106">เมื่อต้องการล้าง Microsoft Teams จากเครื่องเป้าหมายหรือผู้ใช้หลายราย[ให้ดู การล้างข้อมูลการปรับใช้ Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="ad08e-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="ad08e-107">ใช้ [ตัวเลือก PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) เพื่อป้องกันไม่ให้ Microsoft Teams ติดตั้งโดยอัตโนมัติกับ Office</span><span class="sxs-lookup"><span data-stu-id="ad08e-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="ad08e-108">ใช้ [ตัวเลือก PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ก่อนที่จะติดตั้ง Teams* เพื่อป้องกันไม่ให้ Microsoft Teams เริ่มโดยอัตโนมัติหลังจากการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="ad08e-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="ad08e-109">ถ้าคุณใช้งาน Office for Mac ให้ดู[การติดตั้ง Microsoft Teams บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="ad08e-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>