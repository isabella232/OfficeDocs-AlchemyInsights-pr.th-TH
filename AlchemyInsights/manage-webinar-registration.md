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
# <a name="manage-webinar-registration"></a><span data-ttu-id="1371d-102">จัดการการลงทะเบียนการสัมมนาผ่านเว็บ</span><span class="sxs-lookup"><span data-stu-id="1371d-102">Manage webinar registration</span></span>

<span data-ttu-id="1371d-103">คุณสามารถจัดการผู้ที่สามารถลงทะเบียนเข้าร่วมTeamsสัมมนาผ่านเว็บโดยใช้Teamsสั่ง Powershell</span><span class="sxs-lookup"><span data-stu-id="1371d-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="1371d-104">เมื่อต้องการTeams Powershell [Teams PowerShell](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="1371d-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="1371d-105">ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและตั้งค่า **เป็น EveryoneInCompany**</span><span class="sxs-lookup"><span data-stu-id="1371d-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="1371d-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span><span class="sxs-lookup"><span data-stu-id="1371d-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="1371d-107">**หมายเหตุ**: ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้</span><span class="sxs-lookup"><span data-stu-id="1371d-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="1371d-108">เมื่อต้องการเรียนรู้เพิ่มเติมและเปิดใช้งานการตั้งค่านี้[ให้ดู จัดการการตั้งค่าการประชุมใน Microsoft Teams](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="1371d-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="1371d-109">ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ</span><span class="sxs-lookup"><span data-stu-id="1371d-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="1371d-110">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ</span><span class="sxs-lookup"><span data-stu-id="1371d-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="1371d-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="1371d-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
