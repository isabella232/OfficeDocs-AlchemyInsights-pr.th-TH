---
title: เริ่มต้นใช้งานกิจกรรมถ่ายทอดสดของ Teams
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
ms.openlocfilehash: 4b131f7d0cd39070bbc878823a47496bd6b3c99b
ms.sourcegitcommit: fb24e7f90a2c422588da21f54b577d2a178dd344
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/03/2020
ms.locfileid: "43143014"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="cf883-102">เริ่มต้นใช้งานกิจกรรมถ่ายทอดสดของ Teams</span><span class="sxs-lookup"><span data-stu-id="cf883-102">Getting started with Teams live events</span></span>

<span data-ttu-id="cf883-103">เหตุการณ์สดของ Microsoft Teams คือส่วนขยายของการประชุม Teams ที่ช่วยให้คุณสามารถจัดกําหนดการและจัดทําเหตุการณ์ที่สตรีมไปยังผู้ชมออนไลน์ขนาดใหญ่ได้</span><span class="sxs-lookup"><span data-stu-id="cf883-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="cf883-104">ในการสร้างกิจกรรมสด คุณจะต้องมีสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="cf883-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="cf883-105">[สิทธิ์การใช้งาน Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="cf883-105">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="cf883-106">**หมายเหตุ**: เนื่องจากการใช้งาน Teams เพิ่มขึ้นเมื่อเร็วๆ นี้</span><span class="sxs-lookup"><span data-stu-id="cf883-106">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="cf883-107">คุณจะไม่สามารถกําหนดนโยบาย Teams ให้กับ Teams ได้ และอาจไม่มีสิทธิ์เข้าถึงคุณลักษณะบางอย่างของ Teams เช่น การโทรและการประชุมทางเสียง</span><span class="sxs-lookup"><span data-stu-id="cf883-107">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="cf883-108">สิทธิ์ในการ[สร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)</span><span class="sxs-lookup"><span data-stu-id="cf883-108">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="cf883-109">สิทธิ์[ในการสร้างเหตุการณ์สดในสตรีมของ Microsoft](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (สําหรับเหตุการณ์ที่เกิดขึ้นโดยใช้แอปหรืออุปกรณ์กระจายเสียงภายนอก)</span><span class="sxs-lookup"><span data-stu-id="cf883-109">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="cf883-110">สมาชิกในทีมเต็มรูปแบบในองค์กร (ไม่สามารถเป็นแขกหรือจากองค์กรอื่น)</span><span class="sxs-lookup"><span data-stu-id="cf883-110">Full team membership in the org (can't be a guest or from another org).</span></span>

- <span data-ttu-id="cf883-111">การจัดกําหนดการการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP เปิดอยู่ในนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="cf883-111">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="cf883-112">[หลักปฏิบัติที่ดีที่สุด](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42)สําหรับกิจกรรมสดของทีม</span><span class="sxs-lookup"><span data-stu-id="cf883-112">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="cf883-113">สําหรับข้อมูลเพิ่มเติม โปรดดูที่[การเริ่มต้นใช้งานเหตุการณ์การถ่ายทอดสดของ Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)</span><span class="sxs-lookup"><span data-stu-id="cf883-113">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>
