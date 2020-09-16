---
title: บายพาสล็อกการเปิดใช้งานบนอุปกรณ์ iOS ที่มีการดูแลระบบด้วย Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757319"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="52279-102">บายพาสล็อกการเปิดใช้งานบนอุปกรณ์ iOS ที่มีการดูแลระบบด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="52279-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="52279-103">ความสามารถในการเลี่ยงผ่านการล็อกการเปิดใช้งานบนอุปกรณ์ iOS ทำให้ง่ายต่อการกู้คืนจากสถานการณ์ที่ผู้ใช้เปิดใช้งานการล็อกการเปิดใช้งานบนอุปกรณ์ขององค์กรแล้วออกจากบริษัท</span><span class="sxs-lookup"><span data-stu-id="52279-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="52279-104">ก่อน requisites เพื่อข้ามการล็อกการเปิดใช้งานมีดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="52279-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="52279-105">อุปกรณ์คือ "การดูแล"</span><span class="sxs-lookup"><span data-stu-id="52279-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="52279-106">เปิดใช้งานการล็อกการเปิดใช้งานเสร็จเรียบร้อยแล้วโดยใช้นโยบายการจำกัดอุปกรณ์ iOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="52279-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="52279-107">นอกจากนี้เมื่อข้ามการล็อกการเปิดใช้งานคุณควร:</span><span class="sxs-lookup"><span data-stu-id="52279-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="52279-108">ร่างกายมีอุปกรณ์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="52279-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="52279-109">คัดลอกโค้ดก่อนที่คุณจะออกจากการลบ</span><span class="sxs-lookup"><span data-stu-id="52279-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="52279-110">**หมายเหตุ:** รหัสการลบไม่ตรงตามตัวพิมพ์ใหญ่-เล็กดังนั้นไม่จำเป็นต้องมีอักขระ "-"</span><span class="sxs-lookup"><span data-stu-id="52279-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="52279-111">สำหรับรายละเอียดให้ดู[ที่การเปิดใช้งานการล็อกการเปิดใช้งานบนอุปกรณ์ iOS ที่มีการดูแลระบบด้วย Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass)</span><span class="sxs-lookup"><span data-stu-id="52279-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="52279-112">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="52279-112">**FAQ**</span></span>

<span data-ttu-id="52279-113">Q: **ฉันออกการดำเนินการระยะไกลเพื่อเอาข้อมูลบริษัทออกจากอุปกรณ์และตอนนี้จะติดอยู่ในสถานะที่ค้างอยู่**</span><span class="sxs-lookup"><span data-stu-id="52279-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="52279-114">A: สำหรับการดำเนินการระยะไกลเสร็จสมบูรณ์แล้วอุปกรณ์เป้าหมายต้องเป็นแบบออนไลน์และมีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="52279-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="52279-115">ในสถานการณ์ต่อไปนี้การดำเนินการระยะไกลจะยังคงอยู่ในสถานะที่ค้างอยู่เป็นเวลา30วันหรือจนกว่าอุปกรณ์จะได้รับคำสั่งเมื่ออุปกรณ์ดังกล่าวดังนี้</span><span class="sxs-lookup"><span data-stu-id="52279-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="52279-116">ไม่มีการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="52279-116">Does not have connectivity.</span></span>
- <span data-ttu-id="52279-117">สูญเสียสถานะการจัดการด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="52279-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="52279-118">ถ้าคุณคิดว่าอุปกรณ์ไม่ได้รับการตรวจสอบอีกต่อไปและจะไม่เอาข้อมูลบริษัทออกให้เลือกลบ</span><span class="sxs-lookup"><span data-stu-id="52279-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="52279-119">การลบจะเอาระเบียนอุปกรณ์ออกเพื่อไม่ให้ปรากฏในรายการของอุปกรณ์ Intune อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="52279-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="52279-120">สำหรับอุปกรณ์ที่จะเปิดใช้งานอีกครั้งผู้ใช้จะต้องลงทะเบียนอุปกรณ์ใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="52279-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="52279-121">Q: **เหตุใดการดำเนินการระยะไกลบางอย่างจึงไม่พร้อมใช้งานสำหรับฉัน**</span><span class="sxs-lookup"><span data-stu-id="52279-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="52279-122">A: ทุกแพลตฟอร์มการสนับสนุนการดำเนินการอุปกรณ์ระยะไกลทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="52279-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="52279-123">การดำเนินการระยะไกลต่อไปนี้จะเป็นแบบเฉพาะของ platform</span><span class="sxs-lookup"><span data-stu-id="52279-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="52279-124">บายพาสล็อกการเปิดใช้งาน (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="52279-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="52279-125">เริ่มต้นใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="52279-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="52279-126">โหมดสูญหาย (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="52279-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="52279-127">ค้นหาอุปกรณ์ (iOS เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="52279-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="52279-128">เริ่มต้นระบบใหม่ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="52279-128">Restart (Windows only)</span></span>

<span data-ttu-id="52279-129">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการดำเนินการแต่ละรายการให้ดูที่[การดำเนินการของอุปกรณ์ที่พร้อมใช้งาน](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="52279-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>