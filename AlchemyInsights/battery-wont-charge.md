---
title: แบตเตอรี่ไม่ชาร์จ
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
- "9002952"
- "5654"
ms.openlocfilehash: b15939c264a39687b4d93874553e5af7b3f7fe8d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686337"
---
# <a name="battery-wont-charge"></a><span data-ttu-id="dc099-102">แบตเตอรี่ไม่ชาร์จ</span><span class="sxs-lookup"><span data-stu-id="dc099-102">Battery won't charge</span></span>

<span data-ttu-id="dc099-103">ก่อนอื่นให้ตรวจสอบให้แน่ใจว่าการเชื่อมต่อปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="dc099-103">First, make sure connections are secure.</span></span> <span data-ttu-id="dc099-104">เราขอแนะนำให้คุณใช้แหล่งจ่ายไฟเฉพาะ Microsoft หรือที่ได้รับอนุญาตของ Microsoft เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="dc099-104">We strongly recommend that you use only the genuine Microsoft or Microsoft-licensed power supply.</span></span>

<span data-ttu-id="dc099-105">ประการที่สองให้ลองปิด Surface ของคุณและชาร์จเป็นเวลาอย่างน้อย30นาที</span><span class="sxs-lookup"><span data-stu-id="dc099-105">Secondly, try shutting down your Surface and charge for at least 30 minutes.</span></span> <span data-ttu-id="dc099-106">แล้วเปิดอีกครั้งเพื่อดูว่าสามารถแก้ไขปัญหาได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="dc099-106">Then turn it back on to see if that fixes the problem.</span></span>

<span data-ttu-id="dc099-107">**เสียบปลั๊กแต่ไม่ได้ชาร์จ**</span><span class="sxs-lookup"><span data-stu-id="dc099-107">**Plugged in, but not charging**</span></span>

<span data-ttu-id="dc099-108">ถ้าไอคอนแบตเตอรี่บนแถบงานแสดงว่า **เสียบสายไม่ใช่การชาร์จ**นั่นหมายความว่า Surface ของคุณตรวจพบแหล่งจ่ายไฟแต่ยังไม่ได้ชาร์จแบตเตอรี่</span><span class="sxs-lookup"><span data-stu-id="dc099-108">If the battery icon on the taskbar shows **Plugged in, not charging**, it means your Surface detects the power supply but it is not charging the battery.</span></span> <span data-ttu-id="dc099-109">Surface ของคุณอาจปิดใช้งานเมื่อคุณถอดปลั๊กไฟ</span><span class="sxs-lookup"><span data-stu-id="dc099-109">Your Surface may turn off when you unplug it.</span></span> <span data-ttu-id="dc099-110">ลองทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="dc099-110">Try this:</span></span>

1. <span data-ttu-id="dc099-111">เสียบปลั๊ก Surface ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dc099-111">Plug in your Surface.</span></span>
2. <span data-ttu-id="dc099-112">เลือกกล่องค้นหาในแถบงานแล้วพิมพ์ **ตัวจัดการอุปกรณ์**จากนั้นเลือก **ตัวจัดการอุปกรณ์** จากรายการผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="dc099-112">Select the search box in the taskbar, type **device manager**, and then select **Device Manager** from the list of results.</span></span>
3. <span data-ttu-id="dc099-113">คลิกลูกศรที่อยู่ถัดจากประเภท**แบตเตอรี่**</span><span class="sxs-lookup"><span data-stu-id="dc099-113">Click the arrow next to the **Batteries** category.</span></span>
4. <span data-ttu-id="dc099-114">แตะสองครั้งหรือดับเบิลคลิกที่**แบตเตอรี่วิธีการควบคุมที่สอดคล้องกับ ACPI ของไมโครซอฟท์**เลือกแท็บ**โปรแกรมควบคุม**แล้วคลิก**ถอนการติดตั้ง > ตกลง**</span><span class="sxs-lookup"><span data-stu-id="dc099-114">Double-tap or double-click **Microsoft Surface ACPI-Compliant Control Method Battery**, select the **Driver** tab, and click **Uninstall > OK**.</span></span>
5. <span data-ttu-id="dc099-115">เลือกคอมพิวเตอร์ที่อยู่ด้านบนของประเภททั้งหมดเลือกเมนู**การกระทำ**แล้วคลิก**สแกนหาการเปลี่ยนแปลงฮาร์ดแวร์**</span><span class="sxs-lookup"><span data-stu-id="dc099-115">Select the computer at the top of all the categories, select the **Action** menu, and then click **Scan for hardware changes**.</span></span>
6. <span data-ttu-id="dc099-116">ปล่อยให้ Surface ของคุณเสียบปลั๊กไว้</span><span class="sxs-lookup"><span data-stu-id="dc099-116">Leave your Surface plugged in.</span></span>

<span data-ttu-id="dc099-117">หลังจากที่คุณเอาโปรแกรมควบคุมแบตเตอรี่ออกแล้วให้ติดตั้งการอัปเดต Surface และ Windows</span><span class="sxs-lookup"><span data-stu-id="dc099-117">After you remove the battery driver, install Surface and Windows updates.</span></span> <span data-ttu-id="dc099-118">ให้ดูที่ [อัปเดทเฟิร์มแวร์ของ Surface และ Windows 10](https://support.microsoft.com/help/4023505) สำหรับรายละเอียด</span><span class="sxs-lookup"><span data-stu-id="dc099-118">See [Update Surface firmware and Windows 10](https://support.microsoft.com/help/4023505) for details.</span></span> <span data-ttu-id="dc099-119">ตรวจสอบแบตเตอรี่ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dc099-119">Check your battery.</span></span> <span data-ttu-id="dc099-120">ถ้ายังคงมีปัญหาให้ดู[ที่บังคับให้ปิดเครื่องแล้วเริ่มระบบ Surface ของคุณใหม่](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface)</span><span class="sxs-lookup"><span data-stu-id="dc099-120">If it's still having problems, see [Force a shut down and restart your Surface](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface).</span></span>

<span data-ttu-id="dc099-121">**ข้อมูลการแก้ไขปัญหาเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="dc099-121">**More troubleshooting information**</span></span>

<span data-ttu-id="dc099-122">ไฟ LED ควรเปิดเมื่อเสียบสายไฟของคุณเข้ากับ Surface ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dc099-122">The LED light should be on when your power connector is plugged into your Surface.</span></span> <span data-ttu-id="dc099-123">ถ้าปิดกะพริบหรือกะพริบสีขาวโปรดดู[สิ่งที่ต้องทำถ้าแหล่งจ่ายไฟของ Surface หรืออุปกรณ์ชาร์จไม่ทำงาน](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply)</span><span class="sxs-lookup"><span data-stu-id="dc099-123">If it is off, blinking, or flashing white, please check out [What to do if your Surface power supply or charger doesn’t work](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply).</span></span> 

<span data-ttu-id="dc099-124">ถ้าคุณกำลังมีปัญหากับ Surface Book ตรวจสอบให้แน่ใจว่าหน้าจอถูกแนบมากับคีย์บอร์ดอย่างเต็มรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="dc099-124">If you're having problems with your Surface Book, make sure the screen is fully attached to the keyboard.</span></span> <span data-ttu-id="dc099-125">ถ้ายังไม่ชาร์จให้เอาหน้าจอออกและล้างตัวเชื่อมต่อด้วยยางลบดินสอ</span><span class="sxs-lookup"><span data-stu-id="dc099-125">If it still won't charge, remove the screen and clean the connectors with a pencil eraser.</span></span> <span data-ttu-id="dc099-126">นอกจากนี้คุณยังอาจต้องการทำความสะอาดหมุดบนส่วนที่ยาวให้แคบลงของอุปกรณ์ชาร์จที่คุณเสียบเข้ากับ Surface ของคุณและตรวจสอบให้แน่ใจว่าหมุดแห้ง</span><span class="sxs-lookup"><span data-stu-id="dc099-126">You may also want to clean the pins on the long, narrow part of the charger that you plug into your Surface, and make sure the pins are dry.</span></span>

<span data-ttu-id="dc099-127">เมื่อต้องการดูวิธีการแก้ไขปัญหาของแบตเตอรี่เพิ่มเติมโปรดดูที่[แบตเตอรี่ surface ไม่ชาร์จไฟหรือ surface ไม่ทำงานด้วยแบตเตอรี่](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge)</span><span class="sxs-lookup"><span data-stu-id="dc099-127">To see more ways of troubleshooting battery problems, please check out [Surface battery won’t charge or Surface won’t run on battery](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge).</span></span>
