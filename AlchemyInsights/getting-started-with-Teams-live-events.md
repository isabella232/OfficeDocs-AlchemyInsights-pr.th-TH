---
title: การเริ่มต้นใช้งานการถ่ายทอดสดของ Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 6ddb1e74d6c7217303da4f21a3bd71cdab3eb871
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563637"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="7dc26-102">การเริ่มต้นใช้งานการถ่ายทอดสดของ Teams</span><span class="sxs-lookup"><span data-stu-id="7dc26-102">Getting started with Teams live events</span></span>

<span data-ttu-id="7dc26-103">เหตุการณ์ที่เกิดขึ้นจริงของ Microsoft Teams เป็นส่วนขยายของการประชุม Teams ที่ช่วยให้คุณสามารถจัดกําหนดการและผลิตเหตุการณ์ที่สตรีมไปยังผู้ชมออนไลน์ขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="7dc26-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="7dc26-104">ในการสร้างไลฟ์ไลฟ์เหตุการณ์ คุณจะต้องมีสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7dc26-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="7dc26-105">ก่อนอื่น ให้ยืนยันว่า Teams Live Events[พร้อมใช้งานในประเทศและภูมิภาคของคุณ](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability) กิจกรรมสดไม่ได้รับการสนับสนุนในบางประเทศ</span><span class="sxs-lookup"><span data-stu-id="7dc26-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="7dc26-106">หากคุณได้กําหนดสิทธิ์การใช้งานและตั้งค่านโยบายแล้ว แต่ยังไม่สามารถสร้าง Teams Live Event ได้ คุณอาจอยู่ในประเทศหรือภูมิภาคที่ยังไม่มีกิจกรรมถ่ายทอดสด</span><span class="sxs-lookup"><span data-stu-id="7dc26-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="7dc26-107">[สิทธิ์การใช้งาน Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="7dc26-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="7dc26-108">**หมายเหตุ**: เนื่องจากการใช้งาน Teams เพิ่มขึ้นเมื่อไม่นานมานี้ เมื่อคุณมอบหมายสิทธิ์การใช้งาน Teams ให้กับผู้ใช้ อาจใช้เวลาประมาณ 24 ชั่วโมงก่อนที่พวกเขาจะตั้งค่าอย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="7dc26-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="7dc26-109">คุณจะไม่สามารถกําหนดนโยบาย Teams ให้กับพวกเขาได้ และผู้ใช้เหล่านั้นอาจไม่สามารถเข้าถึงคุณลักษณะบางอย่างของ Teams เช่น การโทรและการประชุมทางเสียงได้</span><span class="sxs-lookup"><span data-stu-id="7dc26-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="7dc26-110">สิทธิ์ในการ[สร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)</span><span class="sxs-lookup"><span data-stu-id="7dc26-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="7dc26-111">สิทธิ์ในการ[สร้างเหตุการณ์สดในกระแสข้อมูล Microsoft](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (สําหรับเหตุการณ์ที่เกิดขึ้นโดยใช้โปรแกรมประยุกต์ออกอากาศภายนอกหรืออุปกรณ์)</span><span class="sxs-lookup"><span data-stu-id="7dc26-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="7dc26-112">สมาชิกทีมทั้งหมดในองค์กร (ไม่สามารถเป็นแขกหรือจากองค์กรอื่น)</span><span class="sxs-lookup"><span data-stu-id="7dc26-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="7dc26-113">การตั้งเวลาการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP เปิดอยู่ในนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="7dc26-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="7dc26-114">[แนวทางปฏิบัติที่ดีที่สุด](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42)สําหรับ Teams Live Events</span><span class="sxs-lookup"><span data-stu-id="7dc26-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="7dc26-115">สําหรับข้อมูลเพิ่มเติม โปรดดู[การเริ่มต้นใช้งานเหตุการณ์สดของ Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)</span><span class="sxs-lookup"><span data-stu-id="7dc26-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>