---
title: การแก้ไขปัญหาจอภาพที่มีอยู่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690730"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="40872-102">การแก้ไขปัญหาจอภาพที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="40872-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="40872-103">ลองใช้โซลูชันเหล่านี้เพื่อแก้ไขปัญหาหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="40872-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="40872-104">**รีเฟรชการแสดงผลของจอภาพของคุณ:**</span><span class="sxs-lookup"><span data-stu-id="40872-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="40872-105">กดแป้นต่อไปนี้ในเวลาเดียวกัน: แป้น Windows + Ctrl + Shift + B การทำเช่นนี้จะรีเฟรชการสื่อสารกับโปรแกรมควบคุมกราฟิกของคุณ</span><span class="sxs-lookup"><span data-stu-id="40872-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="40872-106">จอภาพของคุณจะกะพริบ momentarily และกลับมาหลังจากผ่านไปสองสามวินาที</span><span class="sxs-lookup"><span data-stu-id="40872-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="40872-107">**แก้ไขปัญหาฮาร์ดแวร์ของจอภาพ:**</span><span class="sxs-lookup"><span data-stu-id="40872-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="40872-108">ถอดสายเคเบิลที่เชื่อมต่อพีซีของคุณกับจอภาพของคุณแล้วเสียบกลับเข้าไปใหม่</span><span class="sxs-lookup"><span data-stu-id="40872-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="40872-109">ยกเลิกการเชื่อมต่ออุปกรณ์ที่ไม่จำเป็นออกจากพีซีของคุณ (เช่นอะแดปเตอร์หรือแท่นต่อ)</span><span class="sxs-lookup"><span data-stu-id="40872-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="40872-110">**ถ้าคุณเพิ่งติดตั้งการอัปเดตในพีซีของคุณคุณสามารถย้อนกลับโปรแกรมควบคุมการแสดงผลของคุณได้ดังนี้**</span><span class="sxs-lookup"><span data-stu-id="40872-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="40872-111">เลือก **เริ่ม**พิมพ์ **ตัวจัดการอุปกรณ์**แล้วเลือก **ตัวจัดการอุปกรณ์** จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="40872-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="40872-112">ขยายส่วนของ**การ์ดแสดงผล**ให้คลิกขวาที่การ์ดแสดงผลของคุณ Ands เลือก**คุณสมบัติ**</span><span class="sxs-lookup"><span data-stu-id="40872-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="40872-113">นำทางไปยังแท็บ**โปรแกรมควบคุม**แล้วเลือก**ย้อนกลับโปรแกรมควบคุม**</span><span class="sxs-lookup"><span data-stu-id="40872-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="40872-114">หมายเหตุ: ถ้าไม่มีให้ใช้งานหรือเป็นสีเทาให้เลือก **ไม่ใช่** จากตัวเลือกด้านล่างเพื่อย้ายไปยังขั้นตอนถัดไป</span><span class="sxs-lookup"><span data-stu-id="40872-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="40872-115">คุณอาจจำเป็นต้องรีสตาร์ตพีซีของคุณก่อนที่การเปลี่ยนแปลงเหล่านี้จะมีผล</span><span class="sxs-lookup"><span data-stu-id="40872-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="40872-116">**ถอนการติดตั้งและติดตั้งโปรแกรมควบคุมการแสดงผลของคุณใหม่:**</span><span class="sxs-lookup"><span data-stu-id="40872-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="40872-117">เลือก **เริ่ม**พิมพ์ **ตัวจัดการอุปกรณ์**แล้วเลือก **ตัวจัดการอุปกรณ์** จากผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="40872-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="40872-118">ขยายส่วนของ**การ์ดแสดงผล**ให้คลิกขวาที่การ์ดแสดงผลของคุณ Ands เลือก**ถอนการติดตั้งอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="40872-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="40872-119">เลือกกล่องที่อยู่ถัดจาก**ลบซอฟต์แวร์โปรแกรมควบคุมสำหรับอุปกรณ์นี้**แล้วเลือก**ถอนการติดตั้ง**</span><span class="sxs-lookup"><span data-stu-id="40872-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="40872-120">หมายเหตุ: คุณอาจถูกขอให้เริ่มระบบคอมพิวเตอร์ของคุณใหม่ในขั้นตอนนี้</span><span class="sxs-lookup"><span data-stu-id="40872-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="40872-121">ตรวจสอบให้แน่ใจว่าได้จดคำแนะนำที่เหลือก่อนที่คุณจะเริ่มต้นใหม่</span><span class="sxs-lookup"><span data-stu-id="40872-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="40872-122">เปิดตัวจัดการอุปกรณ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="40872-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="40872-123">ขยายส่วนของ**การ์ดแสดงผล**ให้คลิกขวาบนการ์ดแสดงผลของคุณแล้วเลือก**อัปเดตไดรเวอร์**</span><span class="sxs-lookup"><span data-stu-id="40872-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="40872-124">เลือก **ค้นหาสำหรับซอฟต์แวร์โปรแกรมควบคุมการอัปเดตโดยอัตโนมัติ** และทำตามคำแนะนำในการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="40872-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>