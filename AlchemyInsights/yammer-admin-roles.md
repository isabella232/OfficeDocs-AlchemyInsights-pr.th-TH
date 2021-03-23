---
title: เกี่ยวกับผู้ดูแลระบบ Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038127"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="6b436-102">เกี่ยวกับผู้ดูแลระบบ Yammer</span><span class="sxs-lookup"><span data-stu-id="6b436-102">About Yammer admins</span></span>

<span data-ttu-id="6b436-103">**ผู้ดูแลระบบเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="6b436-103">**Network admins**</span></span>

<span data-ttu-id="6b436-104">ผู้ดูแลระบบส่วนกลางจะถูกเลื่อนระดับไปยังบทบาทผู้ดูแลระบบที่ผ่านการตรวจสอบในเครือข่าย Yammer โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="6b436-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="6b436-105">ในกรณีต่อไปนี้ โปรโมชันนี้อาจไม่ถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="6b436-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="6b436-106">มีเครือข่าย Yammer อยู่หลายเครือข่าย และผู้ดูแลระบบลงชื่อเข้าใช้ผิดเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="6b436-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="6b436-107">[การรวมเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) จะต้องเข้าถึงเครือข่าย Yammer เดียว</span><span class="sxs-lookup"><span data-stu-id="6b436-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="6b436-108">Azure PIM จะถูกใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6b436-108">Azure PIM is being used.</span></span> <span data-ttu-id="6b436-109">ผู้ใช้อาจไม่ได้รับการเลื่อนระดับเป็นผู้ดูแลระบบส่วนกลางนานพอที่จะมีโปรโมชันเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="6b436-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="6b436-110">การอัปเดตในอนาคตของ Yammer อาจแก้ไขปัญหานี้ แต่ทางที่ดีที่สุดคือเลื่อนระดับผู้ใช้เป็นผู้ดูแลระบบส่วนกลางด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="6b436-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="6b436-111">มีปัญหาการซิงค์กับเครือข่าย Yammer</span><span class="sxs-lookup"><span data-stu-id="6b436-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="6b436-112">ในกรณีนี้ จะต้องมีการร้องขอการสนับสนุนเพื่อตรวจสอบเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6b436-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="6b436-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="6b436-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="6b436-114">**ผู้ดูแลระบบของกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="6b436-114">**Group admins**</span></span>

<span data-ttu-id="6b436-115">ผู้ดูแลระบบของกลุ่มของกลุ่มที่เชื่อมต่อกับ Microsoft 365 จะถูกซิงค์กับสมาชิกของกลุ่มจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="6b436-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="6b436-116">กลุ่มขนาดใหญ่ การซิงค์นี้อาจใช้เวลาขยายเวลา</span><span class="sxs-lookup"><span data-stu-id="6b436-116">For large groups, this sync can take an extended period.</span></span>
