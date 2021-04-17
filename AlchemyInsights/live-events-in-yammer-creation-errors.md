---
title: เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825534"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="ab788-102">เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer</span><span class="sxs-lookup"><span data-stu-id="ab788-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="ab788-103">**การสร้างเหตุการณ์สดของ Yammer**</span><span class="sxs-lookup"><span data-stu-id="ab788-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="ab788-104">Yammer จะแสดงตัวเลือกในการสร้างเหตุการณ์สดตลอดเวลา</span><span class="sxs-lookup"><span data-stu-id="ab788-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="ab788-105">ในบางกรณี ผู้ใช้อาจไม่ตรงตามข้อเบื้องต้นในการสร้างเหตุการณ์สด และได้รับข้อผิดพลาดเมื่อพวกเขาพยายามสร้างเหตุการณ์นั้น</span><span class="sxs-lookup"><span data-stu-id="ab788-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="ab788-106">รายการด้านล่างครอบคลุมสาเหตุทั่วไปของปัญหานี้และมีวิธีการแก้ไขปัญหาให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="ab788-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="ab788-107">**ใครสามารถสร้างเหตุการณ์สดได้**</span><span class="sxs-lookup"><span data-stu-id="ab788-107">**Who can create live events**</span></span>
- <span data-ttu-id="ab788-108">สิทธิ์การใช้งาน Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5</span><span class="sxs-lookup"><span data-stu-id="ab788-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="ab788-109">สิทธิ์ในการสร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ab788-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="ab788-110">สิทธิ์ในการสร้างเหตุการณ์สดใน Microsoft Stream (เหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)</span><span class="sxs-lookup"><span data-stu-id="ab788-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="ab788-111">การเป็นสมาชิกทีมแบบเต็มในองค์กร (ไม่สามารถเป็นแขกหรือมาจากองค์กรอื่น)</span><span class="sxs-lookup"><span data-stu-id="ab788-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="ab788-112">มีการเปิดการจัดตารางการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP ในนโยบายการประชุมทีม</span><span class="sxs-lookup"><span data-stu-id="ab788-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="ab788-113">**นโยบายการสร้างเหตุการณ์สด**</span><span class="sxs-lookup"><span data-stu-id="ab788-113">**Live event creation policies**</span></span>

<span data-ttu-id="ab788-114">Yammer จะเป็นไปตามนโยบายเหตุการณ์สดที่ตั้งค่าในผู้เช่า Office 365 ของคุณเพื่อสตรีม</span><span class="sxs-lookup"><span data-stu-id="ab788-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="ab788-115">ตามค่าเริ่มต้น ทุกคนในองค์กรของคุณสามารถสร้างเหตุการณ์สดได้</span><span class="sxs-lookup"><span data-stu-id="ab788-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="ab788-116">ผู้ดูแลระบบอาจ [เปลี่ยนแปลงการตั้งค่านี้อาจป้องกันไม่ให้ผู้ใช้สร้างเหตุการณ์](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)สดได้</span><span class="sxs-lookup"><span data-stu-id="ab788-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="ab788-117">It is important to check that users have permissions to create live events if they receive a policy error.</span><span class="sxs-lookup"><span data-stu-id="ab788-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
