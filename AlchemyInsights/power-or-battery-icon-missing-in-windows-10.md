---
title: ไอคอนพลังงานหรือแบตเตอรี่หายไปใน Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: d82994c86126ea9c789e846a74e03794c32c5c3c
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/16/2020
ms.locfileid: "44269518"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="ff3d4-102">ไอคอนพลังงานหรือแบตเตอรี่หายไปใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="ff3d4-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="ff3d4-103">หากอุปกรณ์ Windows 10 ของคุณมีแบตเตอรี่ (เช่น แล็ปท็อปหรือแท็บเล็ต หรือพีซีที่เชื่อมต่อผ่าน USB ไปยัง UPS) โดยปกติไอคอนพลังงาน/แบตเตอรี่จะแสดงในแถบงานใกล้กับนาฬิกา เช่น</span><span class="sxs-lookup"><span data-stu-id="ff3d4-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![ไอคอนแบตเตอรี่](media/battery-icon.png)

<span data-ttu-id="ff3d4-105">หากคุณไม่เห็นไอคอนนี้ แสดงว่าไอคอนนั้นอาจถูกซ่อนไว้</span><span class="sxs-lookup"><span data-stu-id="ff3d4-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="ff3d4-106">ไปที่**[การตั้งค่า>แถบ>การตั้งค่าส่วนบุคคล](ms-settings:taskbar?activationSource=GetHelp)**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="ff3d4-107">ในพื้นที่ แจ้งให้ทราบ ให้คลิก**เลือกไอคอนที่จะปรากฏบนแถบงาน**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="ff3d4-108">จากนั้นค้นหารายการ**Power**ในรายการและสลับการตั้งค่าเป็น**เปิด**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![แสดงไอคอน 'พลังงาน' ในแถบงาน](media/power-icon-on.png)

<span data-ttu-id="ff3d4-110">**การแก้ไขปัญหา**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-110">**Troubleshooting**</span></span>

<span data-ttu-id="ff3d4-111">ถ้าคุณทําตามคําแนะนําข้างต้นและสลับ**พลังงาน**เป็นสีเทาหรือมองไม่เห็น**device manager\*\*\*\*Device Manager**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="ff3d4-112">ภายใต้**แบตเตอรี่**ให้คลิกขวาที่แบตเตอรี่สําหรับอุปกรณ์ของคุณ ให้คลิก**ปิดใช้งาน**แล้วคลิก**ใช่**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="ff3d4-113">รอสักครู่ แล้วคลิกขวาที่แบตเตอรี่ และคลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="ff3d4-114">จากนั้นรีสตาร์ทอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="ff3d4-114">Then restart your device.</span></span>

<span data-ttu-id="ff3d4-115">ถ้าคุณทําตามคําแนะนําข้างต้น แต่ไอคอนแบตเตอรีไม่ปรากฏบนแถบงาน**task manager\*\*\*\*Task Manager**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="ff3d4-116">บนแท็บ**กระบวนการ**ภายใต้**ชื่อ**ให้คลิกขวาที่**Explorer**แล้วคลิก**เริ่มระบบใหม่**</span><span class="sxs-lookup"><span data-stu-id="ff3d4-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
