---
title: ใช้ TeamViewer เพื่อจัดการอุปกรณ์ Intune จากระยะไกล
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798467"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="32ed1-102">ใช้ TeamViewer เพื่อจัดการอุปกรณ์ Intune จากระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="32ed1-103">อุปกรณ์ที่จัดการโดย Intune สามารถจัดการได้จากระยะไกลโดยใช้[TeamViewer](https://www.teamviewer.com/)</span><span class="sxs-lookup"><span data-stu-id="32ed1-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="32ed1-104">เมื่อต้องการดูแล Intune โดยใช้ TeamViewer ให้ใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="32ed1-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="32ed1-105">เริ่มต้นด้วยการขอรับข้อมูลประจำตัวจาก TeamViewer เพื่อตั้งค่าตัวเชื่อมต่อ TeamViewer บน Intune</span><span class="sxs-lookup"><span data-stu-id="32ed1-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="32ed1-106">การดำเนินการนี้จะช่วยให้ผู้ดูแลระบบสามารถใส่ข้อมูลประจำตัวใน UI ตัวเชื่อมต่อ TeamViewer ภายใต้อุปกรณ์การดำเนินการแบบครั้งเดียวเพื่อสร้างลิงก์ระหว่าง Intune และบริการ TeamViewer</span><span class="sxs-lookup"><span data-stu-id="32ed1-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="32ed1-107">**ส่วนที่ 1: เริ่มเซสชันด้วยอุปกรณ์ระยะไกล**</span><span class="sxs-lookup"><span data-stu-id="32ed1-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="32ed1-108">ภายใต้ **อุปกรณ์ทั้งหมด**ให้เลือกอุปกรณ์ที่คุณต้องการเริ่มเซสชันระยะไกลด้วย</span><span class="sxs-lookup"><span data-stu-id="32ed1-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="32ed1-109">จาก **... เพิ่มเติม**ให้เลือก**เซสชันความช่วยเหลือระยะไกลใหม่**</span><span class="sxs-lookup"><span data-stu-id="32ed1-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="32ed1-110">เลือก **ใช่** เพื่อยอมรับว่าคุณต้องการสร้างเซสชันระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="32ed1-111">หลังจากที่การร้องขอ "เริ่มเซสชันระยะไกลใหม่" จะได้รับการยอมรับจากบริการ TeamViewer คุณจะเห็นตัวเลือกในการ **เริ่มการช่วยเหลือระยะไกล** ภายใต้รายละเอียดของบานหน้าต่างภาพรวม (หรือสิ่งที่จำเป็น) สำหรับอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="32ed1-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="32ed1-112">เลือก **ดูเพิ่มเติม** เพื่อขยายบานหน้าต่างและแสดงสถานะความช่วยเหลือระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="32ed1-113">เลือก **เริ่มเซสชันระยะไกล** เพื่อเริ่มเซสชันในด้านผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="32ed1-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="32ed1-114">เลือกดาวน์โหลดไบนารี TeamViewer (Windows) แล้วเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="32ed1-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="32ed1-115">**หมายเหตุ:** คุณสามารถละเว้นหน้าเว็บเบราว์เซอร์ใดก็ได้ที่เปิดอยู่ไปยังเว็บไซต์ TeamViewer</span><span class="sxs-lookup"><span data-stu-id="32ed1-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="32ed1-116">ยอมรับการร้องขอแอป TeamViewer เพื่อทำการเปลี่ยนแปลงบนอุปกรณ์ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="32ed1-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="32ed1-117">แอป TeamViewer จะเริ่มต้นและมีโค้ดเซสชันในการรับรองความถูกต้องของการเชื่อมต่อกับอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="32ed1-118">**ส่วนที่ 2: บนอุปกรณ์ที่มีการกำหนดเป้าหมายสำหรับเซสชันระยะไกล**</span><span class="sxs-lookup"><span data-stu-id="32ed1-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="32ed1-119">เปิดพอร์ทัลบริษัท Intune</span><span class="sxs-lookup"><span data-stu-id="32ed1-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="32ed1-120">ค้นหาค่าสถานะการแจ้งเตือน: "ผู้ดูแลระบบ IT ของคุณกำลังร้องขอการควบคุมอุปกรณ์นี้สำหรับเซสชันความช่วยเหลือระยะไกล" แล้วเลือกการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="32ed1-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="32ed1-121">เลือกดาวน์โหลดแอปพลิเคชัน TeamViewer หรือรับทราบการดาวน์โหลดแอป TeamViewer จาก app store แล้วเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="32ed1-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="32ed1-122">**หมายเหตุ:** คุณสามารถละเว้นหน้าเว็บเบราว์เซอร์ใดก็ได้ที่เปิดอยู่ไปยังเว็บไซต์ TeamViewer</span><span class="sxs-lookup"><span data-stu-id="32ed1-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="32ed1-123">ยอมรับการร้องขอแอป TeamViewer เพื่อทำการเปลี่ยนแปลงบนอุปกรณ์ (เฉพาะ Windows เท่านั้น)</span><span class="sxs-lookup"><span data-stu-id="32ed1-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="32ed1-124">แอป TeamViewer จะเริ่มต้นและมีโค้ดเซสชันในการรับรองความถูกต้องของการเชื่อมต่อกับอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="32ed1-125">ป็อปอัพจะถามว่าคุณต้องการอนุญาตให้เซสชันเริ่มต้นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="32ed1-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="32ed1-126">**หมายเหตุ:** รหัสเซสชันที่สร้างโดยบริการ TeamViewer จะใช้ครั้งเดียวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="32ed1-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="32ed1-127">ถ้าคุณสูญเสียการเชื่อมต่อคุณต้อง:</span><span class="sxs-lookup"><span data-stu-id="32ed1-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="32ed1-128">ปิดอินสแตนซ์ของแอป TeamViewer บนอุปกรณ์ระยะไกลและบนเวิร์กสเตชันผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="32ed1-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="32ed1-129">ปิดพอร์ทัลของบริษัทบนอุปกรณ์ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="32ed1-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="32ed1-130">เริ่มใหม่ "เซสชันความช่วยเหลือระยะไกลใหม่" จากพอร์ทัลการดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="32ed1-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="32ed1-131">เปิดพอร์ทัลของบริษัทบนอุปกรณ์ระยะไกลเพื่อรับการแจ้งเตือนใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="32ed1-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="32ed1-132">ดาวน์โหลดและเปิดแอป TeamViewer บนอุปกรณ์ระยะไกลและเวิร์กสเตชันของผู้ดูแลระบบตามที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="32ed1-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>