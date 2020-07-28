---
title: ค้นหาอุปกรณ์ iOS ที่สูญหายด้วย Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440431"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="b31ae-102">ค้นหาอุปกรณ์ iOS ที่สูญหายด้วย Intun</span><span class="sxs-lookup"><span data-stu-id="b31ae-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="b31ae-103">การเปิดใช้งานโหมดสูญหายบนอุปกรณ์ iOS ทําให้ผู้ดูแลระบบมีข้อความและหมายเลขโทรศัพท์ติดต่อแสดงบนหน้าจอเมื่อล็อก</span><span class="sxs-lookup"><span data-stu-id="b31ae-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="b31ae-104">หลังจากโหมดสูญหายถูกเปิดใช้งานผู้ดูแลระบบสามารถใช้การกระทํา Locate device เพื่อระบุตําแหน่งทางกายภาพของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="b31ae-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="b31ae-105">การกระทําระบุตําแหน่งอุปกรณ์ใน Intuna ทํางานร่วมกับอุปกรณ์ iOS เพื่อแสดงตําแหน่งที่ตั้งของอุปกรณ์ที่ระบุบนแผนที่</span><span class="sxs-lookup"><span data-stu-id="b31ae-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="b31ae-106">การใช้การกระทํานี้ต้องการให้อุปกรณ์ iOS อยู่ใน:</span><span class="sxs-lookup"><span data-stu-id="b31ae-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="b31ae-107">โหมดควบคุม</span><span class="sxs-lookup"><span data-stu-id="b31ae-107">Supervised mode</span></span>
- <span data-ttu-id="b31ae-108">โหมดสูญหาย</span><span class="sxs-lookup"><span data-stu-id="b31ae-108">Lost mode</span></span>

<span data-ttu-id="b31ae-109">ดูข้อมูลเพิ่มเติมได้ที่[เปิดใช้งานโหมดสูญหายบนอุปกรณ์ iOS/iPadOS ด้วย Intuni](https://docs.microsoft.com/intune/device-lost-mode)และ[ค้นหาอุปกรณ์ iOS/iPadOS ที่สูญหายหรือถูกขโมยด้วย Intuni](https://docs.microsoft.com/intune/device-locate)</span><span class="sxs-lookup"><span data-stu-id="b31ae-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="b31ae-110">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="b31ae-110">**FAQ**</span></span>

<span data-ttu-id="b31ae-111">ถาม: ฉันออกการดําเนินการระยะไกลเพื่อลบข้อมูลบริษัทออกจากอุปกรณ์ และตอนนี้ก็ติดอยู่ในสถานะที่รอดําเนินการ</span><span class="sxs-lookup"><span data-stu-id="b31ae-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="b31ae-112">A: เพื่อให้การดําเนินการจากระยะไกลเสร็จสมบูรณ์อุปกรณ์เป้าหมายจะต้องออนไลน์และมีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="b31ae-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="b31ae-113">ในสถานการณ์ต่อไปนี้ การดําเนินการระยะไกลจะอยู่ในสถานะค้างอยู่ 30 วัน หรือจนกว่าอุปกรณ์จะยอมรับคําสั่ง:</span><span class="sxs-lookup"><span data-stu-id="b31ae-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="b31ae-114">เมื่ออุปกรณ์ไม่มีการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="b31ae-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="b31ae-115">เมื่ออุปกรณ์สูญเสียสถานะการจัดการกับ Intun</span><span class="sxs-lookup"><span data-stu-id="b31ae-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="b31ae-116">หากคุณคิดว่าอุปกรณ์ไม่ได้เช็คอินอีกต่อไป และจะไม่สามารถลบข้อมูลของบริษัทออก ได้ ให้เลือก ลบ</span><span class="sxs-lookup"><span data-stu-id="b31ae-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="b31ae-117">การลบจะเอาระเบียนอุปกรณ์ออกเพื่อไม่ให้ปรากฏในรายการอุปกรณ์ Intun</span><span class="sxs-lookup"><span data-stu-id="b31ae-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="b31ae-118">หากอุปกรณ์ทํางานอีกครั้งผู้ใช้จะต้องลงทะเบียนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b31ae-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="b31ae-119">ถาม: เหตุใดการกระทําระยะไกลบางอย่างจึงไม่พร้อมใช้งานสําหรับใช้</span><span class="sxs-lookup"><span data-stu-id="b31ae-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="b31ae-120">A: แพลตฟอร์มทั้งหมดไม่สนับสนุนการกระทําของอุปกรณ์ระยะไกลทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="b31ae-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="b31ae-121">การดําเนินการระยะไกลต่อไปนี้เป็นแพลตฟอร์มเฉพาะ ดังนั้นพวกเขาจะใช้ได้เฉพาะสําหรับแพลตฟอร์มที่ระบุไว้</span><span class="sxs-lookup"><span data-stu-id="b31ae-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="b31ae-122">บายพาสการล็อคการเปิดใช้งาน (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="b31ae-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="b31ae-123">เริ่มต้นใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="b31ae-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="b31ae-124">โหมดสูญหาย (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="b31ae-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="b31ae-125">ค้นหาอุปกรณ์ (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="b31ae-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="b31ae-126">เริ่มระบบใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="b31ae-126">Restart (Windows only)</span></span>

<span data-ttu-id="b31ae-127">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับแต่ละการกระทํา ให้ดูที่[การดําเนินการของอุปกรณ์ที่พร้อมใช้งาน](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="b31ae-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>