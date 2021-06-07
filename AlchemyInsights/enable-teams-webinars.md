---
title: เปิดใช้งานการสัมมนาTeamsผ่านเว็บ
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794037"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="88788-102">เปิดใช้งานการสัมมนาTeamsผ่านเว็บ</span><span class="sxs-lookup"><span data-stu-id="88788-102">Enable Teams Webinars</span></span>

<span data-ttu-id="88788-103">การสัมมนาผ่านเว็บจะเปิดใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="88788-103">Webinars are enabled by default.</span></span> <span data-ttu-id="88788-104">คุณสามารถจัดการผู้ที่สามารถจัดเวลาและลงทะเบียนการสัมมนาผ่านTeamsผ่านเว็บโดยใช้Teams PowerShell ของคุณ</span><span class="sxs-lookup"><span data-stu-id="88788-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="88788-105">ผู้ใช้ทั้งหมดที่สามารถสร้างการประชุมยังสามารถสร้างการประชุมการสัมมนาผ่านเว็บได้</span><span class="sxs-lookup"><span data-stu-id="88788-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="88788-106">ถ้าคุณต้องการจัดการผู้ที่สามารถจัดเวลาการสัมมนาTeamsผ่านเว็บ *ให้ใช้ AllowMeetingRegistration*</span><span class="sxs-lookup"><span data-stu-id="88788-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="88788-107">ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและ **ตั้งค่าเป็น** ทุกคน</span><span class="sxs-lookup"><span data-stu-id="88788-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="88788-108">ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ</span><span class="sxs-lookup"><span data-stu-id="88788-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="88788-109">เมื่อต้องการเปลี่ยนการตั้งค่าเหล่านี้ คุณต้องติดตั้ง[Teams PowerShell](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="88788-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="88788-110">นอกจากนี้ นโยบายการประชุมจะถูกบังคับใช้บนTeamsการสัมมนาผ่านเว็บ</span><span class="sxs-lookup"><span data-stu-id="88788-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="88788-111">ตัวอย่างเช่น ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้</span><span class="sxs-lookup"><span data-stu-id="88788-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="88788-112">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ</span><span class="sxs-lookup"><span data-stu-id="88788-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="88788-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="88788-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>