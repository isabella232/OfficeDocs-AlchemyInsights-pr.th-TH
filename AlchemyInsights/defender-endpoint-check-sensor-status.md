---
title: สถานะเซนเซอร์การตรวจสอบจุดสิ้นสุดของ Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676334"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="939e6-102">สถานะเซนเซอร์การตรวจสอบจุดสิ้นสุดของ Defender</span><span class="sxs-lookup"><span data-stu-id="939e6-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="939e6-103">ไทล์ **ปัญหาเซนเซอร์** อยู่บนแดชบอร์ดการดําเนินการรักษาความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="939e6-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="939e6-104">ไทล์นี้จะให้ข้อมูลเกี่ยวกับความสามารถของอุปกรณ์แต่ละเครื่องในการให้ข้อมูลเซ็นเซอร์และสื่อสารกับ Defender เพื่อบริการจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="939e6-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="939e6-105">รายงานว่าอุปกรณ์ต่างๆ ต้องการการให้ความสนใจกี่เครื่องและช่วยให้คุณระบุอุปกรณ์ที่มีปัญหาและเริ่มแก้ไขปัญหาที่ทราบแล้ว</span><span class="sxs-lookup"><span data-stu-id="939e6-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="939e6-106">ตัวบ่งชี้สถานะสองตัวบนไทล์จะให้ข้อมูลเกี่ยวกับจํานวนอุปกรณ์ที่ไม่ได้รายงานไปยังบริการอย่างถูกต้อง ดังนี้</span><span class="sxs-lookup"><span data-stu-id="939e6-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="939e6-107">**ถูกปรับแต่งผิด** อุปกรณ์ที่อาจรายงานข้อมูลเซ็นเซอร์บางส่วนไปยัง Defender เป็นบริการจุดสิ้นสุด และอาจมีข้อผิดพลาดในการกําหนดค่าที่ต้องมีการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="939e6-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="939e6-108">**ไม่ได้ใช้งาน** อุปกรณ์ที่หยุดการรายงานไปยังบริการ Defender for Endpoint เป็นเวลามากกว่าเจ็ดวันในเดือนที่แล้ว</span><span class="sxs-lookup"><span data-stu-id="939e6-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="939e6-109">การคลิกที่กลุ่มใดกลุ่มหนึ่งจะเลือกคุณไปยังรายการ อุปกรณ์ ที่ถูกกรองตามตัวเลือกของคุณ</span><span class="sxs-lookup"><span data-stu-id="939e6-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="939e6-110">ในรายการ อุปกรณ์ คุณสามารถกรองรายการสถานะความสมบูรณ์ตามสถานะต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="939e6-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="939e6-111">**ใช้งานอยู่** อุปกรณ์ที่รายงานไปยัง Defender อย่างแข็งขันเกี่ยวกับบริการจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="939e6-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="939e6-112">**ถูกปรับแต่งผิด** อุปกรณ์ที่อาจรายงานข้อมูลเซ็นเซอร์บางส่วนไปยัง Defender เป็นบริการจุดสิ้นสุด แต่มีข้อผิดพลาดการกําหนดค่าที่ต้องมีการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="939e6-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="939e6-113">อุปกรณ์ที่ตั้งค่าผิดสามารถมีปัญหาอย่างใดอย่างหนึ่งหรือปัญหาต่อไปนี้รวมกัน:</span><span class="sxs-lookup"><span data-stu-id="939e6-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="939e6-114">ไม่มีข้อมูลเซ็นเซอร์ - อุปกรณ์ได้หยุดส่งข้อมูลเซ็นเซอร์</span><span class="sxs-lookup"><span data-stu-id="939e6-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="939e6-115">การแจ้งเตือนที่จํากัดสามารถทริกเกอร์จากอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="939e6-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="939e6-116">การติดต่อสื่อสารที่มีความบกพร่อง - ความสามารถในการสื่อสารกับอุปกรณ์มีปัญหา</span><span class="sxs-lookup"><span data-stu-id="939e6-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="939e6-117">การส่งไฟล์เพื่อการวิเคราะห์เชิงลึก การบล็อกไฟล์ การแยกอุปกรณ์ออกจากเครือข่ายและการดการดการอื่นๆ ที่ต้องมีการติดต่อสื่อสารกับอุปกรณ์อาจไม่สามารถใช้งาน</span><span class="sxs-lookup"><span data-stu-id="939e6-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="939e6-118">**ไม่ได้ใช้งาน** อุปกรณ์ที่หยุดการรายงานไปยัง Defender ของบริการจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="939e6-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="939e6-119">คุณสามารถดาวน์โหลดรายการทั้งหมดในรูปแบบ CSV โดยใช้ฟีเจอร์ส่งออก</span><span class="sxs-lookup"><span data-stu-id="939e6-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="939e6-120">ดูข้อมูลเพิ่มเติมที่ ตรวจสอบสถานะ[สถานภาพเซ็นเซอร์ใน Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="939e6-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="939e6-121">For more information about what caused a device to be inactive or misconfigured, [see Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="939e6-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
