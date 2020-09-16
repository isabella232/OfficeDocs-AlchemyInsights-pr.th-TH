---
title: ไอคอน Power หรือแบตเตอรีหายไปใน Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 10213843f8ec5ceeaa191d3373406d767f2bea3c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771560"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="c0839-102">ไอคอน Power หรือแบตเตอรีหายไปใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="c0839-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="c0839-103">ถ้าอุปกรณ์ Windows 10 ของคุณมีแบตเตอรี่ (เช่นแล็ปท็อปหรือแท็บเล็ตหรือพีซีที่เชื่อมต่อผ่าน USB กับ UPS) โดยปกติไอคอน power/แบตเตอรี่จะแสดงอยู่ในแถบงานที่อยู่ใกล้กับนาฬิกาตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="c0839-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![ไอคอนแบตเตอรี่](media/battery-icon.png)

<span data-ttu-id="c0839-105">ถ้าคุณไม่เห็นไอคอนนี้แสดงว่าไอคอนดังกล่าวอาจถูกซ่อนไว้:</span><span class="sxs-lookup"><span data-stu-id="c0839-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="c0839-106">ไปที่**[การตั้งค่า > > แถบงานการตั้งค่าส่วนบุคคล](ms-settings:taskbar?activationSource=GetHelp)**</span><span class="sxs-lookup"><span data-stu-id="c0839-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="c0839-107">ในพื้นที่การแจ้งให้ทราบให้คลิก**เลือกไอคอนที่ปรากฏบนแถบงาน**</span><span class="sxs-lookup"><span data-stu-id="c0839-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="c0839-108">จากนั้นค้นหารายการ**พลังงาน**ในรายการและสลับการตั้งค่าเป็น**เปิด**</span><span class="sxs-lookup"><span data-stu-id="c0839-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![แสดงไอคอน power ในแถบงาน](media/power-icon-on.png)

<span data-ttu-id="c0839-110">**การแก้ไขปัญหา**</span><span class="sxs-lookup"><span data-stu-id="c0839-110">**Troubleshooting**</span></span>

<span data-ttu-id="c0839-111">ถ้าคุณทำตามคำแนะนำข้างต้นและสวิตช์ **Power** จะเป็นสีเทาหรือไม่ปรากฏในกล่องค้นหาบนแถบงานให้พิมพ์ **ตัวจัดการอุปกรณ์**แล้วเลือก **ตัวจัดการอุปกรณ์** ในรายการผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="c0839-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="c0839-112">ภายใต้**แบตเตอรี่**ให้คลิกขวาที่แบตเตอรี่สำหรับอุปกรณ์ของคุณแล้วคลิก**ปิดใช้งาน**แล้วคลิก**ใช่**</span><span class="sxs-lookup"><span data-stu-id="c0839-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="c0839-113">รอสองสามวินาทีจากนั้นคลิกขวาที่แบตเตอรี่แล้วคลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="c0839-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="c0839-114">จากนั้นรีสตาร์ตอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="c0839-114">Then restart your device.</span></span>

<span data-ttu-id="c0839-115">ถ้าคุณทำตามคำแนะนำข้างต้นแต่ไอคอนแบตเตอรีไม่ปรากฏบนแถบงานในกล่องค้นหาบนแถบงานให้พิมพ์ **ตัวจัดการงาน**แล้วคลิก **ตัวจัดการงาน** ในรายการผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="c0839-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="c0839-116">บนแท็บ**กระบวนการ**ภายใต้**ชื่อ**ให้คลิกขวาที่**Explorer**แล้วคลิก**เริ่มใหม่**</span><span class="sxs-lookup"><span data-stu-id="c0839-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
