---
title: เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948021"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="7840b-102">เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer</span><span class="sxs-lookup"><span data-stu-id="7840b-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="7840b-103">**การสร้างเหตุการณ์ Yammer สด**</span><span class="sxs-lookup"><span data-stu-id="7840b-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="7840b-104">Yammer จะแสดงตัวเลือกในการสร้างเหตุการณ์สดตลอดเวลา</span><span class="sxs-lookup"><span data-stu-id="7840b-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="7840b-105">ในบางกรณี ผู้ใช้อาจไม่ตรงตามข้อกําหนดเบื้องต้นสําหรับการสร้างเหตุการณ์สด และได้รับข้อผิดพลาดเมื่อพวกเขาพยายามที่จะสร้าง</span><span class="sxs-lookup"><span data-stu-id="7840b-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="7840b-106">รายการด้านล่างครอบคลุมสาเหตุทั่วไปสําหรับปัญหานี้ และให้วิธีการแก้ไขปัญหาสําหรับผู้ใช้ปลายทาง</span><span class="sxs-lookup"><span data-stu-id="7840b-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="7840b-107">**ใครสามารถสร้างกิจกรรมถ่ายทอดสดได้**</span><span class="sxs-lookup"><span data-stu-id="7840b-107">**Who can create live events**</span></span>
- <span data-ttu-id="7840b-108">มี Office 365 องค์กร E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5</span><span class="sxs-lookup"><span data-stu-id="7840b-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="7840b-109">สิทธิ์ในการสร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7840b-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="7840b-110">สิทธิ์ในการสร้างเหตุการณ์สดในสตรีมของ Microsoft (สําหรับเหตุการณ์ที่เกิดขึ้นโดยใช้แอปหรืออุปกรณ์กระจายเสียงภายนอก)</span><span class="sxs-lookup"><span data-stu-id="7840b-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="7840b-111">สมาชิกในทีมเต็มรูปแบบในองค์กร (ไม่สามารถเป็นแขกหรือจากองค์กรอื่น)</span><span class="sxs-lookup"><span data-stu-id="7840b-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="7840b-112">การจัดกําหนดการการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP เปิดอยู่ในนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="7840b-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="7840b-113">**นโยบายการสร้างเหตุการณ์สด**</span><span class="sxs-lookup"><span data-stu-id="7840b-113">**Live event creation policies**</span></span>

<span data-ttu-id="7840b-114">Yammer เป็นไปตามนโยบายเหตุการณ์แบบสดที่ตั้งค่าในผู้เช่า Office 365 ของคุณสําหรับสตรีม</span><span class="sxs-lookup"><span data-stu-id="7840b-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="7840b-115">ตามค่าเริ่มต้น ทุกคนในองค์กรของคุณสามารถสร้างกิจกรรมแบบสดได้</span><span class="sxs-lookup"><span data-stu-id="7840b-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="7840b-116">ผู้ดูแลระบบอาจ[ทําการเปลี่ยนแปลงการตั้งค่านี้ ซึ่งอาจป้องกันไม่ให้ผู้ใช้สร้างเหตุการณ์แบบสด](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)</span><span class="sxs-lookup"><span data-stu-id="7840b-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="7840b-117">สิ่งสําคัญคือต้องตรวจสอบว่าผู้ใช้มีสิทธิ์ในการสร้างเหตุการณ์สดหากได้รับข้อผิดพลาดของนโยบาย</span><span class="sxs-lookup"><span data-stu-id="7840b-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
