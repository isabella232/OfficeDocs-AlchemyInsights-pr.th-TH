---
title: แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755867"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d8f46-102">แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="d8f46-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d8f46-103">ถ้าคุณได้รับข้อผิดพลาด0x8004de40 กับ OneDrive:</span><span class="sxs-lookup"><span data-stu-id="d8f46-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d8f46-104">รีบูตเครื่องคอมพิวเตอร์ที่ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมน Acitve ไดเรกทอรีของคุณ</span><span class="sxs-lookup"><span data-stu-id="d8f46-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d8f46-105">หากการรีบูตไม่สามารถแก้ไขปัญหาได้ให้ยกเลิกการรวมและข้อมูลอุปกรณ์ของคุณจากโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="d8f46-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d8f46-106">**หมายเหตุ**: คุณควรอยู่ในเครือข่ายขององค์กรในขณะที่ทำตามขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="d8f46-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d8f46-107">อย่าทำตามขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรของคุณได้ (ตัวอย่างเช่นขณะเดินทาง)</span><span class="sxs-lookup"><span data-stu-id="d8f46-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d8f46-108">เปิดพร้อมท์คำสั่ง</span><span class="sxs-lookup"><span data-stu-id="d8f46-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d8f46-109">เมื่อต้องการเปิดพร้อมท์คำสั่งให้คลิก-**เริ่ม**คลิกขวาที่**พร้อมท์คำสั่ง**และจากนั้นคลิ**กเรียกใช้ในฐานะผู้ดูแล**</span><span class="sxs-lookup"><span data-stu-id="d8f46-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d8f46-110">พิมพ์*dsregcmd/ปล่อย*และกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="d8f46-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d8f46-111">เมื่อเสร็จสมบูรณ์ให้พิมพ์*dsregcmd/เข้าร่วม*และกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="d8f46-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d8f46-112">เมื่อเสร็จแล้วให้ปิดพรอมต์คำสั่ง</span><span class="sxs-lookup"><span data-stu-id="d8f46-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d8f46-113">รีบูตเครื่องคอมพิวเตอร์และเข้าสู่ระบบไปยัง OneDrive</span><span class="sxs-lookup"><span data-stu-id="d8f46-113">Reboot the computer, and log into OneDrive.</span></span>