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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798663"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="206b8-102">จัดการการลงทะเบียนการสัมมนาผ่านเว็บ</span><span class="sxs-lookup"><span data-stu-id="206b8-102">Manage webinar registration</span></span>

<span data-ttu-id="206b8-103">คุณสามารถจัดการผู้ที่สามารถลงทะเบียนเข้าร่วมTeamsสัมมนาผ่านเว็บโดยใช้Teamsสั่ง Powershell</span><span class="sxs-lookup"><span data-stu-id="206b8-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="206b8-104">เมื่อต้องการTeams Powershell [Teams PowerShell](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="206b8-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="206b8-105">ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและ **ตั้งค่าเป็น** ทุกคน</span><span class="sxs-lookup"><span data-stu-id="206b8-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="206b8-106">ถ้าคุณไม่เห็นตัวเลือกเพื่ออนุญาตการลงทะเบียนให้ทุกคนในคําเชิญเข้าร่วมประชุม ให้เรียกใช้การตั้งค่า *WhoCanRegister ใหม่* เป็น ทุกคน และรอ 24 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="206b8-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="206b8-107">เมื่อต้องการเรียกใช้ *WhoCanRegister ใหม่* ให้ใช้สั่ง Powershell:</span><span class="sxs-lookup"><span data-stu-id="206b8-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="206b8-108">**หมายเหตุ**: ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้</span><span class="sxs-lookup"><span data-stu-id="206b8-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="206b8-109">เมื่อต้องการเรียนรู้เพิ่มเติมและเปิดใช้งานการตั้งค่านี้[ให้ดู จัดการการตั้งค่าการประชุมใน Microsoft Teams](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="206b8-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="206b8-110">ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ</span><span class="sxs-lookup"><span data-stu-id="206b8-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="206b8-111">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ</span><span class="sxs-lookup"><span data-stu-id="206b8-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="206b8-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="206b8-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
