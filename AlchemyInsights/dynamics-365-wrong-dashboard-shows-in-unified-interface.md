---
title: Dynamics ๓๖๕-แสดงแดชบอร์ดที่ไม่ถูกต้องในส่วนติดต่อของ Dynamics ๓๖๕แบบ Unified
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711294"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="96a21-102">แดชบอร์ดที่ไม่ถูกต้องแสดงในส่วนติดต่อแบบ unified ของ Dynamics ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="96a21-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="96a21-103">มีเหตุผลหลายประการที่คุณอาจเห็นแดชบอร์ดอื่นนอกเหนือจากที่คุณคาดหวังว่า:</span><span class="sxs-lookup"><span data-stu-id="96a21-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="96a21-104">ผู้ใช้ได้ตั้งค่าแดชบอร์ดเริ่มต้นของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="96a21-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="96a21-105">โดยปกติแล้วคุณสามารถระบุแดชบอร์ดเริ่มต้นของผู้ใช้ถูกตั้งค่าถ้าปุ่ม **ตั้งค่าเป็นค่าเริ่มต้น** ไม่แสดงในแถบคำสั่งของแดชบอร์ด</span><span class="sxs-lookup"><span data-stu-id="96a21-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="96a21-106">แดชบอร์ดเริ่มต้นของผู้ใช้จะแทนที่แดชบอร์ดเริ่มต้นอื่นๆทั้งหมดแม้ว่าแดชบอร์ดเริ่มต้นของผู้ใช้ไม่ได้อยู่ในแอปปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="96a21-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="96a21-107">ใช้วิธีแก้ไขปัญหาชั่วคราวต่อไปนี้เพื่อเลิกแดชบอร์ดเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="96a21-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="96a21-108">สร้างแดชบอร์ดส่วนบุคคลใหม่</span><span class="sxs-lookup"><span data-stu-id="96a21-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="96a21-109">ตั้งค่าแดชบอร์ดใหม่ให้เป็นค่าเริ่มต้นของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="96a21-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="96a21-110">ลบแดชบอร์ดนั้น</span><span class="sxs-lookup"><span data-stu-id="96a21-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="96a21-111">แดชบอร์ดถูกตั้งค่าในแผนผังเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="96a21-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="96a21-112">คุณอาจตั้งค่าแดชบอร์ดเริ่มต้นขององค์กรโดยการเลือกแดชบอร์ดและเลือก ' ตั้งค่าเป็นค่าเริ่มต้น ' ภายใต้ ' กำหนดระบบ ' เอง</span><span class="sxs-lookup"><span data-stu-id="96a21-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="96a21-113">แต่แดชบอร์ดที่กำหนดไว้ในตัวออกแบบแผนผังเว็บไซต์จะมีความสำคัญเหนือแดชบอร์ดนี้ถ้าผู้ใช้มีสิทธิ์เข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="96a21-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="96a21-114">เมื่อต้องการให้ผู้ใช้เห็นแดชบอร์ดที่คุณได้ตั้งค่าเป็นค่าเริ่มต้นขององค์กรคุณสามารถทำได้ดังนี้</span><span class="sxs-lookup"><span data-stu-id="96a21-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="96a21-115">ตั้งค่าแดชบอร์ดนั้นในแผนผังเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="96a21-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="96a21-116">เอาการเข้าถึงแดชบอร์ดที่กำหนดเองของแผนผังของผู้ใช้เหล่านั้นออก</span><span class="sxs-lookup"><span data-stu-id="96a21-116">Remove access to the sitemap defined dashboard for those users</span></span>
