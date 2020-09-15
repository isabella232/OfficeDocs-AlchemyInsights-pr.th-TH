---
title: การค้นหาอุปกรณ์ iOS ที่สูญหายด้วย Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675199"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="2c6cb-102">การค้นหาอุปกรณ์ iOS ที่สูญหายด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="2c6cb-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="2c6cb-103">การเปิดใช้งานโหมดสูญหายบนอุปกรณ์ iOS จะช่วยให้ผู้ดูแลระบบสามารถใส่ข้อความและหมายเลขโทรศัพท์ที่ติดต่อที่แสดงบนหน้าจอเมื่อล็อกได้</span><span class="sxs-lookup"><span data-stu-id="2c6cb-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="2c6cb-104">หลังจากที่โหมดสูญหายถูกเปิดใช้งานผู้ดูแลระบบสามารถใช้การดำเนินการค้นหาอุปกรณ์เพื่อระบุตำแหน่งที่ตั้งทางกายภาพของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2c6cb-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="2c6cb-105">การดำเนินการค้นหาอุปกรณ์ใน Intune ทำงานกับอุปกรณ์ iOS เพื่อแสดงตำแหน่งที่ตั้งของอุปกรณ์ที่เฉพาะเจาะจงบนแผนที่</span><span class="sxs-lookup"><span data-stu-id="2c6cb-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="2c6cb-106">การใช้การกระทำนี้จำเป็นต้องใช้อุปกรณ์ iOS ในการดำเนินการดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="2c6cb-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="2c6cb-107">โหมดการดูแล</span><span class="sxs-lookup"><span data-stu-id="2c6cb-107">Supervised mode</span></span>
- <span data-ttu-id="2c6cb-108">โหมดสูญหาย</span><span class="sxs-lookup"><span data-stu-id="2c6cb-108">Lost mode</span></span>

<span data-ttu-id="2c6cb-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่[เปิดใช้งานโหมดสูญหายบนอุปกรณ์ ios/iPadOS ด้วย intune](https://docs.microsoft.com/intune/device-lost-mode)และ[ค้นหาอุปกรณ์ iOS/iPadOS ที่สูญหายหรือถูกขโมยด้วย intune](https://docs.microsoft.com/intune/device-locate)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="2c6cb-110">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="2c6cb-110">**FAQ**</span></span>

<span data-ttu-id="2c6cb-111">Q: ฉันออกการดำเนินการระยะไกลเพื่อเอาข้อมูลบริษัทออกจากอุปกรณ์และตอนนี้จะติดอยู่ในสถานะที่ค้างอยู่</span><span class="sxs-lookup"><span data-stu-id="2c6cb-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="2c6cb-112">A: สำหรับการดำเนินการระยะไกลเสร็จสมบูรณ์แล้วอุปกรณ์เป้าหมายต้องเป็นแบบออนไลน์และมีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="2c6cb-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="2c6cb-113">ในสถานการณ์ต่อไปนี้การดำเนินการระยะไกลจะยังคงอยู่ในสถานะที่ค้างอยู่เป็นเวลา30วันหรือจนกว่าอุปกรณ์จะยอมรับคำสั่งดังนี้</span><span class="sxs-lookup"><span data-stu-id="2c6cb-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="2c6cb-114">เมื่ออุปกรณ์ไม่มีการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="2c6cb-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="2c6cb-115">เมื่ออุปกรณ์สูญเสียสถานะการจัดการด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="2c6cb-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="2c6cb-116">ถ้าคุณคิดว่าอุปกรณ์ไม่ได้รับการตรวจสอบอีกต่อไปและจะไม่สามารถเอาข้อมูลบริษัทออกได้ให้เลือกลบ</span><span class="sxs-lookup"><span data-stu-id="2c6cb-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="2c6cb-117">การลบจะเอาระเบียนอุปกรณ์ออกเพื่อไม่ให้ปรากฏในรายการของอุปกรณ์ Intune อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="2c6cb-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="2c6cb-118">ถ้าอุปกรณ์เปิดใช้งานอีกครั้งผู้ใช้จะต้องลงทะเบียนใหม่</span><span class="sxs-lookup"><span data-stu-id="2c6cb-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="2c6cb-119">Q: เหตุใดการดำเนินการระยะไกลบางอย่างจึงไม่พร้อมใช้งานสำหรับฉัน</span><span class="sxs-lookup"><span data-stu-id="2c6cb-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="2c6cb-120">A: ทุกแพลตฟอร์มการสนับสนุนการดำเนินการอุปกรณ์ระยะไกลทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="2c6cb-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="2c6cb-121">การดำเนินการระยะไกลต่อไปนี้จะเป็นแบบเฉพาะสำหรับแพลตฟอร์มดังนั้นพวกเขาจะพร้อมใช้งานสำหรับแพลตฟอร์มที่ระบุไว้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="2c6cb-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="2c6cb-122">บายพาสล็อกการเปิดใช้งาน (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="2c6cb-123">เริ่มต้นใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="2c6cb-124">โหมดสูญหาย (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="2c6cb-125">ค้นหาอุปกรณ์ (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="2c6cb-126">เริ่มต้นระบบใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-126">Restart (Windows only)</span></span>

<span data-ttu-id="2c6cb-127">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการดำเนินการแต่ละรายการให้ดูที่[การดำเนินการของอุปกรณ์ที่พร้อมใช้งาน](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="2c6cb-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>