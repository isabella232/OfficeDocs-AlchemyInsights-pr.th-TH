---
title: การแก้ไขปัญหาจอภาพที่มีอยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738587"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="7a825-102">การแก้ไขปัญหาจอภาพที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="7a825-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="7a825-103">ลองใช้โซลูชันเหล่านี้เพื่อแก้ไขปัญหาจอภาพ</span><span class="sxs-lookup"><span data-stu-id="7a825-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="7a825-104">**รีเฟรชจอแสดงผลของจอภาพ:**</span><span class="sxs-lookup"><span data-stu-id="7a825-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="7a825-105">กดปุ่มต่อไปนี้ในเวลาเดียวกัน: Windows คีย์ + Ctrl + Shift + B การทำเช่นนี้จะรีเฟรชการสื่อสารกับโปรแกรมควบคุมกราฟิกของคุณ</span><span class="sxs-lookup"><span data-stu-id="7a825-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="7a825-106">จอภาพของคุณจะกะพริบอย่างรวดเร็วและกลับมาหลังจากนั้นไม่กี่วินาที</span><span class="sxs-lookup"><span data-stu-id="7a825-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="7a825-107">**การแก้ไขปัญหาฮาร์ดแวร์การตรวจสอบ:**</span><span class="sxs-lookup"><span data-stu-id="7a825-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="7a825-108">ถอดสายเคเบิลที่เชื่อมต่อพีซีของคุณเข้ากับจอภาพแล้วเสียบกลับเข้าไปใหม่</span><span class="sxs-lookup"><span data-stu-id="7a825-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="7a825-109">ยกเลิกการเชื่อมต่ออุปกรณ์ที่ไม่จำเป็นใดๆจากพีซีของคุณ (เช่นอะแดปเตอร์หรือแท่นวาง)</span><span class="sxs-lookup"><span data-stu-id="7a825-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="7a825-110">**หากคุณเพิ่งติดตั้งการอัปเดตในพีซีของคุณคุณสามารถย้อนกลับโปรแกรมควบคุมจอแสดงผลของคุณได้:**</span><span class="sxs-lookup"><span data-stu-id="7a825-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="7a825-111">เลือก**เริ่มต้น**พิมพ์**ตัวจัดการอุปกรณ์**และเลือก**ตัวจัดการอุปกรณ์**จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="7a825-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7a825-112">ขยายส่วน**การ์ดแสดงผล**คลิกขวา**ที่**อะแดปเตอร์จอแสดงผลของคุณ</span><span class="sxs-lookup"><span data-stu-id="7a825-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="7a825-113">นำทางไปยังแท็บ**โปรแกรมควบคุม**และเลือก**ย้อนกลับไดรเวอร์**</span><span class="sxs-lookup"><span data-stu-id="7a825-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="7a825-114">หมายเหตุ: หากไม่สามารถใช้งานได้หรือเป็นสีเทาให้เลือก**No**จากตัวเลือกด้านล่างเพื่อย้ายไปยังขั้นตอนถัดไป</span><span class="sxs-lookup"><span data-stu-id="7a825-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="7a825-115">คุณอาจต้องรีสตาร์ทเครื่องคอมพิวเตอร์ก่อนที่การเปลี่ยนแปลงเหล่านี้จะมีผล</span><span class="sxs-lookup"><span data-stu-id="7a825-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="7a825-116">**ถอนการติดตั้งและติดตั้งโปรแกรมควบคุมจอแสดงผลของคุณใหม่:**</span><span class="sxs-lookup"><span data-stu-id="7a825-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="7a825-117">เลือก**เริ่มต้น**พิมพ์**ตัวจัดการอุปกรณ์**และเลือก**ตัวจัดการอุปกรณ์**จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="7a825-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7a825-118">ขยายส่วน**การ์ดแสดงผล**คลิกขวาที่การ์ดแสดงผลของคุณเลือก**ถอนการติดตั้งอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="7a825-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="7a825-119">เลือกกล่องที่อยู่ถัดจาก**ลบซอฟต์แวร์โปรแกรมควบคุมสำหรับอุปกรณ์นี้**แล้วเลือก**ถอนการติดตั้ง**</span><span class="sxs-lookup"><span data-stu-id="7a825-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="7a825-120">หมายเหตุ: ระบบอาจขอให้คุณรีสตาร์ทเครื่องคอมพิวเตอร์ในขั้นตอนนี้</span><span class="sxs-lookup"><span data-stu-id="7a825-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="7a825-121">ตรวจสอบให้แน่ใจว่าได้จดคำแนะนำที่เหลือก่อนที่คุณจะเริ่มต้นใหม่</span><span class="sxs-lookup"><span data-stu-id="7a825-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="7a825-122">เปิดตัวจัดการอุปกรณ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7a825-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="7a825-123">ขยายส่วน**การ์ดแสดงผล**คลิกขวาบนการ์ดแสดงผลของคุณและเลือก**ปรับปรุงโปรแกรมควบคุม**</span><span class="sxs-lookup"><span data-stu-id="7a825-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="7a825-124">เลือก**ค้นหาโดยอัตโนมัติสำหรับซอฟต์แวร์โปรแกรมควบคุมการปรับปรุง**และทำตามคำแนะนำการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="7a825-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>