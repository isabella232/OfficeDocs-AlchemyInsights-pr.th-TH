---
title: การเริ่มต้นใช้งานการแข่งขันที่มีอยู่ในทีม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677298"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="017f8-102">การเริ่มต้นใช้งานการแข่งขันที่มีอยู่ในทีม</span><span class="sxs-lookup"><span data-stu-id="017f8-102">Getting started with Teams live events</span></span>

<span data-ttu-id="017f8-103">เหตุการณ์ live team ของ Microsoft เป็นส่วนขยายของการประชุมทีมที่ช่วยให้คุณสามารถจัดกำหนดการและสร้างเหตุการณ์ที่สตรีมไปยังผู้ชมออนไลน์ขนาดใหญ่ได้</span><span class="sxs-lookup"><span data-stu-id="017f8-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="017f8-104">เมื่อต้องการสร้างเหตุการณ์สดคุณจะต้องมีสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="017f8-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="017f8-105">ก่อนอื่นให้ตรวจสอบว่าทีมเหตุการณ์สด [พร้อมใช้งานในประเทศและภูมิภาคของคุณ](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability) เหตุการณ์สดยังไม่ได้รับการสนับสนุนในบางประเทศ</span><span class="sxs-lookup"><span data-stu-id="017f8-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="017f8-106">ถ้าคุณได้กำหนดสิทธิ์การใช้งานและตั้งค่านโยบายแล้วแต่ยังไม่สามารถสร้างทีมเหตุการณ์ที่ถ่ายทอดสดได้อาจเป็นไปได้ว่าคุณอยู่ในประเทศหรือภูมิภาคที่ยังไม่พร้อมใช้งานเหตุการณ์ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="017f8-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="017f8-107">[สิทธิ์การใช้งาน office ๓๖๕ Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน office ๓๖๕ A3 หรือ A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="017f8-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="017f8-108">**หมายเหตุ**: เนื่องจากการเพิ่มขึ้นของการใช้งานของทีมเมื่อคุณกำหนดสิทธิ์การใช้งานของทีมให้กับผู้ใช้อาจใช้เวลาประมาณ24ชั่วโมงก่อนที่จะตั้งค่าทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="017f8-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="017f8-109">จากนั้นคุณจะไม่สามารถกำหนดนโยบายของทีมให้กับบุคคลเหล่านั้นได้และอาจไม่สามารถเข้าถึงฟีเจอร์บางอย่างของทีมเช่นการโทรและการประชุมทางเสียงได้</span><span class="sxs-lookup"><span data-stu-id="017f8-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="017f8-110">สิทธิ์ในการ[สร้างเหตุการณ์สดในศูนย์การจัดการทีมของ Microsoft](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)</span><span class="sxs-lookup"><span data-stu-id="017f8-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="017f8-111">สิทธิ์ในการ [สร้างเหตุการณ์สดใน Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (สำหรับเหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)</span><span class="sxs-lookup"><span data-stu-id="017f8-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="017f8-112">การเป็นสมาชิกทีมแบบเต็มรูปแบบในองค์กร (ไม่สามารถเป็นผู้เยี่ยมชมหรือจากองค์กรอื่นได้)</span><span class="sxs-lookup"><span data-stu-id="017f8-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="017f8-113">การจัดกำหนดการการประชุมส่วนตัวการจัดกำหนดการ screensharing และการแชร์วิดีโอ IP เปิดอยู่ในนโยบายการประชุมทีม</span><span class="sxs-lookup"><span data-stu-id="017f8-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="017f8-114">[หลักปฏิบัติที่ดีที่สุด](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) สำหรับการแข่งขันที่มีอยู่ในทีม</span><span class="sxs-lookup"><span data-stu-id="017f8-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="017f8-115">สำหรับข้อมูลเพิ่มเติมโปรดดู[ที่เริ่มต้นใช้งาน Microsoft team live เหตุการณ์](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)</span><span class="sxs-lookup"><span data-stu-id="017f8-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>