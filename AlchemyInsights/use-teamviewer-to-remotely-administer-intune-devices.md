---
title: ใช้ TeamViewer เพื่อจัดการอุปกรณ์ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555752"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="a7765-102">ใช้ TeamViewer เพื่อจัดการอุปกรณ์ Intun</span><span class="sxs-lookup"><span data-stu-id="a7765-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="a7765-103">อุปกรณ์ที่จัดการโดย Intunine สามารถจัดการจากระยะไกลโดยใช้[TeamViewer](https://www.teamviewer.com/)</span><span class="sxs-lookup"><span data-stu-id="a7765-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="a7765-104">เมื่อต้องการจัดการ Intuner โดยใช้ TeamViewer ใช้ขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="a7765-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="a7765-105">เริ่มต้น โดยการรับข้อมูลประจําตัวจาก TeamViewer เพื่อตั้งค่าตัวเชื่อมต่อ TeamViewer บน Intun</span><span class="sxs-lookup"><span data-stu-id="a7765-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="a7765-106">การดําเนินการเพียงครั้งเดียวเพื่อสร้างการเชื่อมโยงระหว่าง Intunen และ TeamViewer บริการ</span><span class="sxs-lookup"><span data-stu-id="a7765-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="a7765-107">**ส่วนที่ 1: เริ่มเซสชันด้วยอุปกรณ์ระยะไกล**</span><span class="sxs-lookup"><span data-stu-id="a7765-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="a7765-108">ภายใต้**อุปกรณ์ทั้งหมด**ให้เลือกอุปกรณ์ที่คุณต้องการเริ่มเซสชันระยะไกลด้วย</span><span class="sxs-lookup"><span data-stu-id="a7765-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="a7765-109">จาก **... เพิ่มเติม**ให้เลือก**เซสชันความช่วยเหลือระยะไกลใหม่**</span><span class="sxs-lookup"><span data-stu-id="a7765-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="a7765-110">เลือก**ใช่**เพื่อรับทราบว่าคุณต้องการสร้างเซสชันระยะไกล</span><span class="sxs-lookup"><span data-stu-id="a7765-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="a7765-111">หลังจากการร้องขอ "การเริ่มต้นเซสชันระยะไกลใหม่" ได้รับการยอมรับโดยบริการ TeamViewer คุณจะเห็นตัวเลือกในการ**เริ่มความช่วยเหลือระยะไกล**ภายใต้รายละเอียดของบานหน้าต่างภาพรวม (หรือสิ่งจําเป็นสําหรับ) สําหรับอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a7765-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="a7765-112">เลือก**ดูเพิ่มเติม**เพื่อขยายบานหน้าต่างและแสดงสถานะ 'ความช่วยเหลือระยะไกล'</span><span class="sxs-lookup"><span data-stu-id="a7765-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="a7765-113">เลือก**เริ่มเซสชันระยะไกล**เพื่อเริ่มเซสชันบนด้านผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="a7765-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="a7765-114">เลือกเพื่อดาวน์โหลดไบนารี TeamViewer (Windows)**และเลือก**</span><span class="sxs-lookup"><span data-stu-id="a7765-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="a7765-115">**หมายเหตุ** คุณสามารถละเว้นหน้าเว็บใดๆ ที่เปิดไปยังเว็บไซต์ TeamViewer ได้</span><span class="sxs-lookup"><span data-stu-id="a7765-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="a7765-116">ยอมรับคําขอสําหรับโปรแกรมประยุกต์ TeamViewer เพื่อทําการเปลี่ยนแปลงบนอุปกรณ์ (Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="a7765-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="a7765-117">แอพลิเคชัน TeamViewer เริ่มต้น และรวมถึงรหัสเซสชันการรับรองความถูกต้องการเชื่อมต่อกับอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="a7765-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="a7765-118">**ส่วนที่ 2: บนอุปกรณ์ที่ถูกกําหนดเป้าหมายสําหรับเซสชันระยะไกล**</span><span class="sxs-lookup"><span data-stu-id="a7765-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="a7765-119">เปิดพอร์ทัลบริษัท Intun</span><span class="sxs-lookup"><span data-stu-id="a7765-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="a7765-120">มองหาธงการแจ้งเตือน: "ผู้ดูแลระบบ IT ของคุณร้องขอการควบคุมอุปกรณ์นี้สําหรับเซสชันความช่วยเหลือระยะไกล" และเลือกการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="a7765-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="a7765-121">เลือกดาวน์โหลดแอปพลิเคชัน TeamViewer หรือรับทราบการดาวน์โหลดแอป TeamViewer จาก App Store แล้วเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="a7765-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="a7765-122">**หมายเหตุ** คุณสามารถละเว้นหน้าเว็บใดๆ ที่เปิดไปยังเว็บไซต์ TeamViewer ได้</span><span class="sxs-lookup"><span data-stu-id="a7765-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="a7765-123">ยอมรับคําขอสําหรับโปรแกรมประยุกต์ TeamViewer เพื่อทําการเปลี่ยนแปลงบนอุปกรณ์ (Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="a7765-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="a7765-124">แอพลิเคชัน TeamViewer เริ่มต้น และรวมถึงรหัสเซสชันการรับรองความถูกต้องการเชื่อมต่อกับอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="a7765-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="a7765-125">ป๊อปอัปจะถามว่าคุณต้องการอนุญาตให้เซสชันเริ่มทํางานหรือไม่</span><span class="sxs-lookup"><span data-stu-id="a7765-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="a7765-126">**หมายเหตุ** รหัสเซสชันที่สร้างขึ้นโดยบริการ TeamViewer จะใช้ครั้งเดียวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="a7765-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="a7765-127">ถ้าคุณสูญเสียการเชื่อมต่อ คุณต้อง:</span><span class="sxs-lookup"><span data-stu-id="a7765-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="a7765-128">ปิดอินสแตนซ์ของโปรแกรมประยุกต์ TeamViewer บนอุปกรณ์ระยะไกล และ บนเวิร์กสเตชันของผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="a7765-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="a7765-129">ปิดพอร์ทัลบริษัทบนอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="a7765-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="a7765-130">เริ่มต้น "เซสชันความช่วยเหลือระยะไกลใหม่" จากพอร์ทัลผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="a7765-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="a7765-131">เปิดพอร์ทัลบริษัทบนอุปกรณ์ระยะไกลอีกครั้งเพื่อรับการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="a7765-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="a7765-132">ดาวน์โหลดและเปิดแอป TeamViewer บนอุปกรณ์ระยะไกลและเวิร์กสเตชันผู้ดูแลระบบเช่นเดียวกับก่อนหน้านี้</span><span class="sxs-lookup"><span data-stu-id="a7765-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>