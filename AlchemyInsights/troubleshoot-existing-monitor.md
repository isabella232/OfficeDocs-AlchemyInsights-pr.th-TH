---
title: การแก้ไขปัญหาจอภาพที่มีอยู่
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824598"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="92318-102">แก้ไขปัญหาจอภาพที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="92318-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="92318-103">ลองโซลูชันเหล่านี้เพื่อแก้ไขปัญหาเกี่ยวกับจอภาพ</span><span class="sxs-lookup"><span data-stu-id="92318-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="92318-104">**รีเฟรชการแสดงผลของจอภาพของคุณ:**</span><span class="sxs-lookup"><span data-stu-id="92318-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="92318-105">กดแป้นต่อไปนี้พร้อมกัน: แป้น Windows + Ctrl + Shift + B การรีเฟรชการติดต่อสื่อสารกับโปรแกรมควบคุมกราฟิกของคุณ</span><span class="sxs-lookup"><span data-stu-id="92318-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="92318-106">หน้าจอของคุณจะกะพริบสักครู่และกลับมาหลังจากผ่านไปสองสามวินาที</span><span class="sxs-lookup"><span data-stu-id="92318-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="92318-107">**แก้ไขปัญหาฮาร์ดแวร์ของจอภาพ:**</span><span class="sxs-lookup"><span data-stu-id="92318-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="92318-108">ถอดสายเคเบิลที่เชื่อมต่อพีซีของคุณเข้ากับจอภาพ และเสียบกลับเข้าอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="92318-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="92318-109">ยกเลิกการเชื่อมต่ออุปกรณ์ที่ไม่เป็นอุปกรณ์ใดๆ จากพีซีของคุณ (เช่น อะแดปเตอร์ หรือแท่นเชื่อมต่อ)</span><span class="sxs-lookup"><span data-stu-id="92318-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="92318-110">**หากคุณเพิ่งติดตั้งการอัปเดตบนพีซี คุณสามารถย้อนกลับโปรแกรมควบคุมการแสดงผลของคุณ:**</span><span class="sxs-lookup"><span data-stu-id="92318-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="92318-111">เลือกเริ่มต้น พิมพ์ **ตัวจัดการ** อุปกรณ์ แล้วเลือก **ตัวจัดการ** อุปกรณ์ จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="92318-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="92318-112">ขยาย **ส่วน การ์ดแสดงผล** คลิกขวาที่การ์ดแสดงผลของคุณ **แล้วเลือก** คุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="92318-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="92318-113">นําทาง **ไปยัง** แท็บ โปรแกรมควบคุม และเลือก **ย้อนกลับโปรแกรมควบคุม**</span><span class="sxs-lookup"><span data-stu-id="92318-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="92318-114">หมายเหตุ: ถ้าตัวเลือกนี้ไม่พร้อมใช้งานหรือเป็นสีเทา **ให้เลือก** ไม่ใช่ จากตัวเลือกด้านล่างเพื่อย้ายไปยังขั้นตอนถัดไป</span><span class="sxs-lookup"><span data-stu-id="92318-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="92318-115">คุณอาจต้องรีสตาร์ตพีซีของคุณก่อนการเปลี่ยนแปลงเหล่านี้จะมีผล</span><span class="sxs-lookup"><span data-stu-id="92318-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="92318-116">**ถอนการติดตั้งและติดตั้งโปรแกรมควบคุมการแสดงผลของคุณอีกครั้ง:**</span><span class="sxs-lookup"><span data-stu-id="92318-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="92318-117">เลือกเริ่มต้น พิมพ์ **ตัวจัดการ** อุปกรณ์ แล้วเลือก **ตัวจัดการ** อุปกรณ์ จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="92318-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="92318-118">ขยาย **ส่วน การ์ดแสดงผล** คลิกขวาที่การ์ดแสดงผลของคุณ แล้วเลือก **ถอนการติดตั้ง** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="92318-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="92318-119">เลือกกล่องที่อยู่ถัดจาก **ลบซอฟต์แวร์โปรแกรมควบคุมบนอุปกรณ์** นี้ **และเลือก** ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="92318-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="92318-120">หมายเหตุ: คุณอาจถูกขอให้รีสตาร์ตคอมพิวเตอร์ในขั้นตอนนี้</span><span class="sxs-lookup"><span data-stu-id="92318-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="92318-121">ตรวจสอบให้แน่ใจว่าได้เขียนคําแนะนําที่เหลือก่อนที่คุณจะเริ่มใหม่</span><span class="sxs-lookup"><span data-stu-id="92318-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="92318-122">เปิดตัวจัดการอุปกรณ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="92318-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="92318-123">ขยาย **ส่วน การ์ดแสดงผล** คลิกขวาบนการ์ดแสดงผลของคุณ แล้วเลือก **อัปเดตโปรแกรมควบคุม**</span><span class="sxs-lookup"><span data-stu-id="92318-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="92318-124">เลือก **ค้นหาซอฟต์แวร์โปรแกรมควบคุมการอัปเดตโดยอัตโนมัติ และปฏิบัติตาม** คําแนะนําในการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="92318-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>