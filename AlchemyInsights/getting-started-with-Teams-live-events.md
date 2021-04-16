---
title: เริ่มต้นใช้งานเหตุการณ์สดของ Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811979"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="e7b64-102">เริ่มต้นใช้งานเหตุการณ์สดของ Teams</span><span class="sxs-lookup"><span data-stu-id="e7b64-102">Getting started with Teams live events</span></span>

<span data-ttu-id="e7b64-103">เหตุการณ์สดของ Microsoft Teams เป็นส่วนขยายของการประชุม Teams ที่ช่วยให้คุณจัดเวลาและสร้างเหตุการณ์ที่สตรีมไปยังผู้ชมออนไลน์ขนาดใหญ่ได้</span><span class="sxs-lookup"><span data-stu-id="e7b64-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="e7b64-104">เมื่อต้องการสร้างเหตุการณ์สด คุณจะต้องมีสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e7b64-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="e7b64-105">ก่อนอื่นให้ยืนยันว่า Teams Live Events [พร้อมให้บริการในประเทศและภูมิภาค](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability)ของคุณ กิจกรรมสดยังไม่ได้รับการสนับสนุนในบางประเทศ</span><span class="sxs-lookup"><span data-stu-id="e7b64-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="e7b64-106">หากคุณได้มอบหมายสิทธิ์การใช้งานและตั้งค่านโยบายแล้ว แต่ยังไม่สามารถสร้างเหตุการณ์สดของ Teams ได้ อาจดูเหมือนว่าคุณอยู่ในประเทศหรือภูมิภาคที่ยังไม่มีเหตุการณ์สด</span><span class="sxs-lookup"><span data-stu-id="e7b64-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="e7b64-107">สิทธิ์การใช้งาน[Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="e7b64-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="e7b64-108">**หมายเหตุ**: เนื่องจากการใช้งาน Teams เพิ่มขึ้นล่าสุด เมื่อคุณกําหนดสิทธิ์การใช้งาน Teams ให้กับผู้ใช้ อาจใช้เวลาประมาณ 24 ชั่วโมงก่อนที่พวกเขาจะตั้งค่าได้อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="e7b64-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="e7b64-109">จนกว่าจะถึงตอนนี้ คุณจะไม่สามารถกําหนดนโยบาย Teams ให้กับพวกเขาได้ และพวกเขาอาจไม่สามารถเข้าถึงฟีเจอร์บางอย่างของ Teams เช่น การโทรและการประชุมผ่านเสียงได้</span><span class="sxs-lookup"><span data-stu-id="e7b64-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="e7b64-110">สิทธิ์ในการ[สร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)</span><span class="sxs-lookup"><span data-stu-id="e7b64-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="e7b64-111">สิทธิ์ในการสร้าง [เหตุการณ์สดใน Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (เหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)</span><span class="sxs-lookup"><span data-stu-id="e7b64-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="e7b64-112">การเป็นสมาชิกทีมแบบเต็มในองค์กร (ไม่สามารถเป็นแขกหรือมาจากองค์กรอื่น)</span><span class="sxs-lookup"><span data-stu-id="e7b64-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="e7b64-113">มีการเปิดการจัดตารางการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP ในนโยบายการประชุมทีม</span><span class="sxs-lookup"><span data-stu-id="e7b64-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="e7b64-114">[แนวทางปฏิบัติที่ดีที่สุด](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) เกี่ยวกับเหตุการณ์สดของ Teams</span><span class="sxs-lookup"><span data-stu-id="e7b64-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="e7b64-115">หากต้องการข้อมูลเพิ่มเติม โปรดดู[เริ่มต้นใช้งานกิจกรรมสดของ Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)</span><span class="sxs-lookup"><span data-stu-id="e7b64-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>