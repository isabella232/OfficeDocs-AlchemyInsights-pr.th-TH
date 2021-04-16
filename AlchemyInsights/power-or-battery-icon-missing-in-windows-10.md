---
title: ไอคอนพลังงานหรือแบตเตอรี่หายไปใน Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790567"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="39cfa-102">ไอคอนพลังงานหรือแบตเตอรี่หายไปใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="39cfa-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="39cfa-103">หากอุปกรณ์ Windows 10 ของคุณมีแบตเตอรี่ (เช่น แล็ปท็อปหรือแท็บเล็ต หรือพีซีที่เชื่อมต่อผ่าน USB กับ UPS) ปกติแล้วไอคอนพลังงาน/แบตเตอรี่จะแสดงอยู่ในแถบงานใกล้กับนาฬิกา ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="39cfa-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![ไอคอนแบตเตอรี่](media/battery-icon.png)

<span data-ttu-id="39cfa-105">ถ้าคุณไม่เห็นไอคอนนี้ ไอคอนอาจซ่อนอยู่:</span><span class="sxs-lookup"><span data-stu-id="39cfa-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="39cfa-106">ไปที่ **[การตั้งค่า >การตั้งค่าส่วนบุคคล >แถบงาน](ms-settings:taskbar?activationSource=GetHelp)**</span><span class="sxs-lookup"><span data-stu-id="39cfa-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="39cfa-107">ในพื้นที่ การแจ้งให้ทราบ **ให้คลิก เลือกไอคอนที่ปรากฏบน** แถบงาน</span><span class="sxs-lookup"><span data-stu-id="39cfa-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="39cfa-108">จากนั้นค้นหา **รายการ** เปิด/ปิดเครื่องในรายการ และสลับการตั้งค่า **เป็น** เปิด</span><span class="sxs-lookup"><span data-stu-id="39cfa-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![แสดงไอคอนเปิด/ปิดเครื่องในแถบงาน](media/power-icon-on.png)

<span data-ttu-id="39cfa-110">**การแก้ไขปัญหา**</span><span class="sxs-lookup"><span data-stu-id="39cfa-110">**Troubleshooting**</span></span>

<span data-ttu-id="39cfa-111">ถ้าคุณปฏิบัติตามคําแนะนําด้านบนและปุ่มสลับเปิด/ปิดเครื่องเป็นสีเทาหรือไม่สามารถมองเห็นได้ ในกล่องค้นหาบนแถบงาน ให้พิมพ์ ตัวจัดการอุปกรณ์ แล้วเลือก **ตัวจัดการ** อุปกรณ์ ในรายการผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="39cfa-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="39cfa-112">**ภายใต้ แบตเตอรี่** ให้คลิกขวาที่แบตเตอรี่ของอุปกรณ์ของคุณ **คลิก** ปิดใช้งาน **แล้วคลิก** ใช่</span><span class="sxs-lookup"><span data-stu-id="39cfa-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="39cfa-113">รอประมาณสองสามวินาที จากนั้นคลิกขวาที่แบตเตอรี่ **แล้วคลิก** เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="39cfa-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="39cfa-114">จากนั้นรีสตาร์ตอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="39cfa-114">Then restart your device.</span></span>

<span data-ttu-id="39cfa-115">ถ้าคุณปฏิบัติตามคําแนะนําด้านบน แต่ไอคอนแบตเตอรี่ไม่ปรากฏบนแถบงาน ในกล่องค้นหาบนแถบงาน พิมพ์ ตัวจัดการงาน **แล้วคลิก** ตัวจัดการงาน ในรายการผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="39cfa-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="39cfa-116">บนแท็บ **กระบวนการ** ภายใต้ ชื่อ **คลิกขวาที่** **Explorer** แล้วคลิก รี **สตาร์** ต</span><span class="sxs-lookup"><span data-stu-id="39cfa-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
