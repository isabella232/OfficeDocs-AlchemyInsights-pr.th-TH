---
title: สร้างและจัดการแท็กหรือกลุ่มอุปกรณ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731970"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="bc2d0-102">สร้างและจัดการแท็กหรือกลุ่มอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="bc2d0-103">เพิ่มแท็กบนอุปกรณ์เพื่อสร้างสังกัดกลุ่มแบบตรรกะ</span><span class="sxs-lookup"><span data-stu-id="bc2d0-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="bc2d0-104">แท็กอุปกรณ์สนับสนุนการแมปเครือข่ายที่เหมาะสม ซึ่งช่วยให้คุณสามารถแนบแท็กต่างๆ เพื่อจัดเก็บบริบทและเพื่อเปิดใช้งานการสร้างรายการแบบไดนามิกเป็นส่วนหนึ่งของเหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="bc2d0-105">แท็กสามารถใช้เป็นตัวกรองในมุมมองรายการอุปกรณ์ หรือเพื่อจัดกลุ่มอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="bc2d0-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="bc2d0-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="bc2d0-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="bc2d0-107">คุณสามารถเพิ่มแท็กบนอุปกรณ์ได้โดย:</span><span class="sxs-lookup"><span data-stu-id="bc2d0-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="bc2d0-108">การใช้พอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="bc2d0-108">Using the portal</span></span>

- <span data-ttu-id="bc2d0-109">การตั้งค่ารีจิสทรีคีย์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-109">Setting a registry key value</span></span>
 
<span data-ttu-id="bc2d0-110">**หมายเหตุ:** อาจมีเวลาแฝงระหว่างเวลาที่แท็กถูกเพิ่มลงในอุปกรณ์และความพร้อมใช้งานในรายการอุปกรณ์และหน้าอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="bc2d0-111">เมื่อต้องการเพิ่มแท็กอุปกรณ์โดยใช้ API ให้ดู[เพิ่มหรือเอาแท็กอุปกรณ์ออก API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="bc2d0-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="bc2d0-112">เพิ่มและจัดการแท็กอุปกรณ์โดยใช้พอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="bc2d0-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="bc2d0-113">เลือกอุปกรณ์ที่คุณต้องการจัดการแท็ก</span><span class="sxs-lookup"><span data-stu-id="bc2d0-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="bc2d0-114">คุณสามารถเลือกหรือค้นหาอุปกรณ์จากมุมมองต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bc2d0-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="bc2d0-115">**แดชบอร์ดการดําเนินการรักษาความปลอดภัย** เลือกชื่ออุปกรณ์จากส่วน อุปกรณ์ยอดนิยมที่มีการแจ้งเตือนที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="bc2d0-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="bc2d0-116">**คิวการแจ้งเตือน** - เลือกชื่ออุปกรณ์ที่อยู่ด้านข้างไอคอนอุปกรณ์จากคิวการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="bc2d0-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="bc2d0-117">**รายการ** อุปกรณ์ - เลือกชื่ออุปกรณ์จากรายการอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="bc2d0-118">**กล่องค้นหา** - เลือกอุปกรณ์ จากเมนูดรอปดาวน์แล้วใส่ชื่ออุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="bc2d0-119">คุณยังสามารถไปที่หน้าการแจ้งเตือนผ่านมุมมองไฟล์และ IP</span><span class="sxs-lookup"><span data-stu-id="bc2d0-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="bc2d0-120">เลือก **จัดการแท็ก** จากแถวของการแอคชันตอบกลับ</span><span class="sxs-lookup"><span data-stu-id="bc2d0-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="bc2d0-121">พิมพ์เพื่อค้นหาหรือสร้างแท็ก</span><span class="sxs-lookup"><span data-stu-id="bc2d0-121">Type to find or create tags.</span></span>

<span data-ttu-id="bc2d0-122">แท็กจะถูกเพิ่มลงในมุมมองอุปกรณ์ และจะปรากฏในมุมมองรายการอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="bc2d0-123">จากนั้นคุณสามารถใช้ตัวกรอง แท็ก เพื่อดูรายการของอุปกรณ์ที่เกี่ยวข้องได้</span><span class="sxs-lookup"><span data-stu-id="bc2d0-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="bc2d0-124">ดูข้อมูลเพิ่มเติมที่ [สร้างและจัดการแท็ก](/microsoft-365/security/defender-endpoint/machine-tags)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bc2d0-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>