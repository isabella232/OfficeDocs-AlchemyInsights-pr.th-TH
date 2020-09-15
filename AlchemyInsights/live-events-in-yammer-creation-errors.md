---
title: เหตุการณ์สดในข้อผิดพลาดการสร้าง Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675461"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="a617c-102">เหตุการณ์สดในข้อผิดพลาดการสร้าง Yammer</span><span class="sxs-lookup"><span data-stu-id="a617c-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="a617c-103">**การสร้างเหตุการณ์ของ Yammer Live**</span><span class="sxs-lookup"><span data-stu-id="a617c-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="a617c-104">Yammer จะแสดงตัวเลือกในการสร้างเหตุการณ์สดตลอดเวลา</span><span class="sxs-lookup"><span data-stu-id="a617c-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="a617c-105">ในบางกรณีผู้ใช้อาจไม่ตรงตามข้อกำหนดเบื้องต้นสำหรับการสร้างเหตุการณ์สดและได้รับข้อผิดพลาดเมื่อพวกเขาพยายามสร้างเหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="a617c-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="a617c-106">รายการต่อไปนี้จะครอบคลุมเหตุผลทั่วไปสำหรับปัญหานี้และให้วิธีการแก้ไขปัญหาสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a617c-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="a617c-107">**ใครสามารถสร้างเหตุการณ์สด**</span><span class="sxs-lookup"><span data-stu-id="a617c-107">**Who can create live events**</span></span>
- <span data-ttu-id="a617c-108">สิทธิ์การใช้งาน Office ๓๖๕ Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office ๓๖๕ A3 หรือ A5</span><span class="sxs-lookup"><span data-stu-id="a617c-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="a617c-109">สิทธิ์ในการสร้างเหตุการณ์สดในศูนย์การจัดการทีมของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a617c-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="a617c-110">สิทธิ์ในการสร้างเหตุการณ์สดใน Microsoft Stream (สำหรับเหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)</span><span class="sxs-lookup"><span data-stu-id="a617c-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="a617c-111">การเป็นสมาชิกทีมแบบเต็มรูปแบบในองค์กร (ไม่สามารถเป็นผู้เยี่ยมชมหรือจากองค์กรอื่นได้)</span><span class="sxs-lookup"><span data-stu-id="a617c-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="a617c-112">การจัดกำหนดการการประชุมส่วนตัวการจัดกำหนดการ screensharing และการแชร์วิดีโอ IP เปิดอยู่ในนโยบายการประชุมทีม</span><span class="sxs-lookup"><span data-stu-id="a617c-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="a617c-113">**นโยบายการสร้างเหตุการณ์แบบสด**</span><span class="sxs-lookup"><span data-stu-id="a617c-113">**Live event creation policies**</span></span>

<span data-ttu-id="a617c-114">Yammer จะติดตามนโยบายเหตุการณ์สดที่ตั้งค่าไว้ในผู้เช่า Office ๓๖๕สำหรับสตรีมของคุณ</span><span class="sxs-lookup"><span data-stu-id="a617c-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="a617c-115">ตามค่าเริ่มต้นทุกคนในองค์กรของคุณสามารถสร้างเหตุการณ์สดได้</span><span class="sxs-lookup"><span data-stu-id="a617c-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="a617c-116">ผู้ดูแลระบบอาจ [ทำการเปลี่ยนแปลงการตั้งค่านี้ซึ่งอาจทำให้ผู้ใช้สร้างเหตุการณ์สด](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)ได้</span><span class="sxs-lookup"><span data-stu-id="a617c-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="a617c-117">คุณจำเป็นต้องตรวจสอบว่าผู้ใช้มีสิทธิ์ในการสร้างเหตุการณ์สดถ้าพวกเขาได้รับข้อผิดพลาดเกี่ยวกับนโยบายหรือไม่</span><span class="sxs-lookup"><span data-stu-id="a617c-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
