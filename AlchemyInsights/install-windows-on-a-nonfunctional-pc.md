---
title: ติดตั้ง Windows บนพีซีที่ไม่ใช่อุปกรณ์
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
- "9001473"
- "3501"
ms.openlocfilehash: e741b99dcc01aaabce001c8b8fe45161a1d3badd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832005"
---
# <a name="install-windows-on-a-nonfunctional-pc"></a><span data-ttu-id="2e176-102">ติดตั้ง Windows บนพีซีที่ไม่ใช่อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2e176-102">Install Windows on a nonfunctional PC</span></span>

<span data-ttu-id="2e176-103">คุณสามารถใช้สื่อการติดตั้ง (แฟลชไดรฟ์ USB หรือดีวีดี) เพื่อติดตั้งสําเนา Windows ใหม่ ติดตั้งใหม่ หรือติดตั้ง Windows ใหม่</span><span class="sxs-lookup"><span data-stu-id="2e176-103">You can use installation media (a USB flash drive or DVD) to install a new copy of Windows, perform a clean installation, or reinstall Windows.</span></span>

1. <span data-ttu-id="2e176-104">**ค้นหาคีย์ผลิตภัณฑ์หรือใบอนุญาตใช้งานดิจิทัล** ของคุณ</span><span class="sxs-lookup"><span data-stu-id="2e176-104">**Locate your product key or digital license**.</span></span>

    - <span data-ttu-id="2e176-105">จะค้นหาคีย์ผลิตภัณฑ์ได้ที่ไหนขึ้นอยู่กับวิธีที่คุณดาวน์โหลดสําเนา Windows</span><span class="sxs-lookup"><span data-stu-id="2e176-105">Where to find your product key depends on how you got your copy of Windows.</span></span> <span data-ttu-id="2e176-106">หากต้องการความช่วยเหลือในการค้นหาผลิตภัณฑ์ ของคุณ ให้ดู [ค้นหาคีย์ผลิตภัณฑ์ Windows](https://support.microsoft.com/help/10749/windows-10-find-product-key)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="2e176-106">For help locating yours, see [Find your Windows product key](https://support.microsoft.com/help/10749/windows-10-find-product-key).</span></span> 

2. <span data-ttu-id="2e176-107">**ใช้ USB แฟลชไดรฟ์หรือดีวีดีเพื่อสร้างสื่อการติดตั้ง** ของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="2e176-107">**Use a USB flash drive or DVD to create your own installation media**.</span></span>

    - <span data-ttu-id="2e176-108">คุณต้องมีคอมพิวเตอร์ที่มีฟังก์ชันการฟังก์ชันแยกต่างหากในขั้นตอนนี้ หากพีซีที่ได้รับ Windows ไม่มีฟังก์ชัน</span><span class="sxs-lookup"><span data-stu-id="2e176-108">You need a separate functioning computer to do this step if the PC to receive Windows is nonfunctional.</span></span>

    - <span data-ttu-id="2e176-109">เราขอแนะนนะให้ใช้ USB เปล่าหรือดีวีดีเปล่าเป็นสื่อการติดตั้ง เนื่องจากเนื้อหาใดๆ ในสื่อจะถูกลบ</span><span class="sxs-lookup"><span data-stu-id="2e176-109">We recommend using a blank USB or blank DVD as the installation media because any content on it will be deleted.</span></span>

    - <span data-ttu-id="2e176-110">ถ้าคุณต้องการจัดรูปแบบไดรฟ์ USB ให้ดู ติดตั้ง [Windows จาก USB แฟลชไดรฟ์](https://docs.microsoft.com/windows-hardware/manufacture/desktop/install-windows-from-a-usb-flash-drive) เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="2e176-110">If you need to format your USB drive, see [Install Windows from a USB Flash Drive](https://docs.microsoft.com/windows-hardware/manufacture/desktop/install-windows-from-a-usb-flash-drive) for more information.</span></span>

    - <span data-ttu-id="2e176-111">เมื่อคุณพร้อมที่จะสร้างสื่อการติดตั้ง ให้ [ดาวน์โหลดและเรียกใช้เครื่องมือการสร้าง](https://www.microsoft.com/software-download/windows10)สื่อ</span><span class="sxs-lookup"><span data-stu-id="2e176-111">When you are ready to create an installation media, [download and run the media creation tool](https://www.microsoft.com/software-download/windows10).</span></span> <span data-ttu-id="2e176-112">ดูคําแนะนําที่นั่นเพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับวิธีการใช้เครื่องมือ</span><span class="sxs-lookup"><span data-stu-id="2e176-112">See the instructions there for more information on how to use the tool.</span></span>

3. <span data-ttu-id="2e176-113">**ติดตั้ง Windows ลงในพีซีที่ไม่ใช่อุปกรณ์ที่ใช้ USB แฟลชไดรฟ์หรือดีวีดีจากขั้นตอนที่ 2**</span><span class="sxs-lookup"><span data-stu-id="2e176-113">**Install Windows to a nonfunctional PC using your USB flash drive or DVD from Step 2**.</span></span>

    - <span data-ttu-id="2e176-114">เชื่อมต่อสื่อการติดตั้งที่คุณสร้างกับพีซีที่ไม่มีขั้นตอน แล้วเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2e176-114">Connect the installation media you created to your nonfunctional PC; then turn it on.</span></span>

    - <span data-ttu-id="2e176-115">บนหน้าจอการตั้งค่าเริ่มต้น ให้ใส่ภาษาและลักษณะอื่นๆ ของคุณ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="2e176-115">On the initial setup screen, enter your language and other preferences and click **Next**.</span></span> <span data-ttu-id="2e176-116">หากคุณไม่เห็นหน้าจอการตั้งค่า พีซีของคุณอาจไม่ได้ตั้งค่าให้เริ่มต้นระบบจากไดรฟ์</span><span class="sxs-lookup"><span data-stu-id="2e176-116">If you don't see the setup screen, your PC might not be set up to boot from a drive.</span></span> <span data-ttu-id="2e176-117">ตรวจสอบเว็บไซต์ของผู้ผลิตพีซีของคุณเพื่อดูข้อมูลเกี่ยวกับวิธีเปลี่ยนล8งการเริ่มต้นระบบของพีซีของคุณ แล้วลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="2e176-117">Check your PC manufacturer's website for info on how to change your PC's boot order, and then try again.</span></span>

    - <span data-ttu-id="2e176-118">คลิก **ซ่อมแซมคอมพิวเตอร์** ของคุณ</span><span class="sxs-lookup"><span data-stu-id="2e176-118">Click **Repair your computer**.</span></span>

    - <span data-ttu-id="2e176-119">บนหน้าจอ **เลือกตัวเลือก\*\*\*\*ให้คลิก** แก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="2e176-119">On the **Choose an option** screen, click **Troubleshoot**.</span></span> <span data-ttu-id="2e176-120">จากที่นั่น คุณสามารถคืนค่าจากจุดคืนค่าระบบได้</span><span class="sxs-lookup"><span data-stu-id="2e176-120">From there, you can restore from a system restore point.</span></span>

<span data-ttu-id="2e176-121">**สิ่ง** สําคัญ: หากคุณพยายามติดตั้ง Windows บนพีซีที่ใช้งานได้ คุณอาจใช้ขั้นตอนที่ 3 แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="2e176-121">**Important**: if you are trying to install Windows on a functional PC, you may do Step 3 differently.</span></span> <span data-ttu-id="2e176-122">หากต้องการคําแนะนําเพิ่มเติมเกี่ยวกับสถานการณ์ต่างๆ[ให้ดูตัวเลือกการกู้คืนใน Windows 10](https://support.microsoft.com/help/12415/windows-10-recovery-options)</span><span class="sxs-lookup"><span data-stu-id="2e176-122">For further instructions on different scenarios, see [Recovery options in Windows 10](https://support.microsoft.com/help/12415/windows-10-recovery-options).</span></span>
