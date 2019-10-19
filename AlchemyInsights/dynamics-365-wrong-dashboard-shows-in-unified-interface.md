---
title: Dynamics ๓๖๕-แดชบอร์ดไม่ถูกต้องแสดงใน Dynamics ๓๖๕อินเทอร์เฟซแบบรวม
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528570"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="bbcea-102">แสดงแดชบอร์ดที่ไม่ถูกต้องในอินเทอร์เฟซแบบรวมของ Dynamics ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="bbcea-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="bbcea-103">มีหลายสาเหตุที่คุณอาจเห็นแดชบอร์ดที่แตกต่างจากที่คุณคาดไว้:</span><span class="sxs-lookup"><span data-stu-id="bbcea-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="bbcea-104">ผู้ใช้ได้ตั้งค่าแดชบอร์ดเริ่มต้นของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="bbcea-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="bbcea-105">โดยปกติแล้วคุณสามารถระบุได้ว่าแดชบอร์ดเริ่มต้นของผู้ใช้ถูกตั้งค่าไว้ถ้าปุ่ม**ตั้งค่าเป็นค่าเริ่มต้น**ไม่แสดงในแถบคำสั่งของแดชบอร์ด</span><span class="sxs-lookup"><span data-stu-id="bbcea-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="bbcea-106">แดชบอร์ดเริ่มต้นของผู้ใช้จะแทนที่แดชบอร์ดเริ่มต้นอื่นๆทั้งหมดแม้ว่าแดชบอร์ดเริ่มต้นของผู้ใช้ไม่ได้อยู่ในแอปปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="bbcea-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="bbcea-107">ใช้วิธีแก้ปัญหาต่อไปนี้เพื่อยกเลิกการตั้งค่าแดชบอร์ดเริ่มต้นของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="bbcea-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="bbcea-108">สร้างแดชบอร์ดส่วนบุคคลใหม่</span><span class="sxs-lookup"><span data-stu-id="bbcea-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="bbcea-109">ตั้งค่าแดชบอร์ดใหม่เป็นค่าเริ่มต้นของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="bbcea-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="bbcea-110">ลบแดชบอร์ดนั้น</span><span class="sxs-lookup"><span data-stu-id="bbcea-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="bbcea-111">แดชบอร์ดถูกตั้งค่าในแผนผังไซต์</span><span class="sxs-lookup"><span data-stu-id="bbcea-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="bbcea-112">คุณอาจตั้งค่าแดชบอร์ดเริ่มต้นขององค์กรโดยการเลือกแดชบอร์ดและเลือก ' ตั้งค่าเป็นค่าเริ่มต้น ' ภายใต้ ' ปรับแต่งระบบ '</span><span class="sxs-lookup"><span data-stu-id="bbcea-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="bbcea-113">แต่แดชบอร์ดที่กำหนดไว้ในโปรแกรมออกแบบแผนผังไซต์จะมีความสำคัญเหนือแดชบอร์ดนี้ถ้าผู้ใช้เข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="bbcea-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="bbcea-114">เมื่อต้องการให้ผู้ใช้เห็นแดชบอร์ดที่คุณตั้งค่าเป็นค่าเริ่มต้นขององค์กรคุณสามารถทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="bbcea-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="bbcea-115">ตั้งค่าแดชบอร์ดที่อยู่ในแผนผังไซต์</span><span class="sxs-lookup"><span data-stu-id="bbcea-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="bbcea-116">ลบสิทธิ์เข้าถึงแดชบอร์ดที่กำหนดแผนผังไซต์สำหรับผู้ใช้เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="bbcea-116">Remove access to the sitemap defined dashboard for those users</span></span>
