---
title: ติดอยู่ในกล่องขาออกเนื่องจากสิ่งที่แนบมาที่มีขนาดใหญ่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241271"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="38b19-102">แก้ไขข้อความที่ติดอยู่ในกล่องขาออก</span><span class="sxs-lookup"><span data-stu-id="38b19-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="38b19-103">เราขอแนะนําให้ คุณเริ่มการทํางาน โดยการเรียกใช้สถานการณ์สมมติ["ฉันมีปัญหาในการส่ง รับ หรือค้นหาข้อความอีเมล"](https://aka.ms/SaRA-OutlookSendReceive)จากเครื่องมือ[สนับสนุนฝ่ายสนับสนุนและกู้คืนของ Microsoft](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="38b19-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="38b19-104">เมื่อข้อความถูกติดอยู่ในกล่องจดหมายออกของคุณ</span><span class="sxs-lookup"><span data-stu-id="38b19-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="38b19-105">**เอาสิ่งที่แนบมาขนาดใหญ่ออก**</span><span class="sxs-lookup"><span data-stu-id="38b19-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="38b19-106">ใน Outlook ให้เลือก**ส่ง / รับ** > **งานแบบออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="38b19-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="38b19-107">ในบานหน้าต่างนําทาง ให้เลือก**กล่องขาออก**</span><span class="sxs-lookup"><span data-stu-id="38b19-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="38b19-108">จากที่นี่ คุณสามารถ:</span><span class="sxs-lookup"><span data-stu-id="38b19-108">From here, you can:</span></span> 
    - <span data-ttu-id="38b19-109">ลบข้อความ (เลือกข้อความนั้น แล้วเลือก**ลบ**)</span><span class="sxs-lookup"><span data-stu-id="38b19-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="38b19-110">ลากข้อความไปยังโฟลเดอร์แบบร่างของคุณ**Delete**</span><span class="sxs-lookup"><span data-stu-id="38b19-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="38b19-111">ถ้าคุณได้รับข้อความแสดงข้อผิดพลาดที่ระบุว่า Outlook กําลังพยายามส่งข้อความ ให้ปิด Outlook</span><span class="sxs-lookup"><span data-stu-id="38b19-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="38b19-112">มันอาจใช้เวลาสักครู่เพื่อออกจาก</span><span class="sxs-lookup"><span data-stu-id="38b19-112">It may take a few moments to exit.</span></span> <span data-ttu-id="38b19-113">ถ้า Outlook ไม่ปิด ให้กด Ctrl+Alt+Delete แล้วเลือก**เริ่มตัวจัดการงาน**</span><span class="sxs-lookup"><span data-stu-id="38b19-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="38b19-114">ใน ตัวจัดการงาน ให้เลือกแท็บ**กระบวนการ**เลื่อนลงไปที่ outlook.exe แล้วเลือก**สิ้นสุด Process**</span><span class="sxs-lookup"><span data-stu-id="38b19-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="38b19-115">หลังจาก Outlook ปิดแล้ว ให้เริ่มใหม่และทําซ้ําขั้นตอนที่ 2 และ 3</span><span class="sxs-lookup"><span data-stu-id="38b19-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="38b19-116">หลังจากที่คุณเอาสิ่งที่แนบมาออก ให้คลิก**ส่ง /** > **รับงานแบบออฟไลน์**เพื่อทํางานแบบออนไลน์ต่อ</span><span class="sxs-lookup"><span data-stu-id="38b19-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="38b19-117">ข้อความยังติดอยู่ในกล่องขาออกเมื่อคุณคลิก**ส่ง**แต่คุณไม่ได้เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="38b19-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="38b19-118">คลิก**ส่ง / รับ**และดูที่ ปุ่ม**ทํางานแบบออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="38b19-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="38b19-119">ถ้าเป็นสีน้ําเงิน</span><span class="sxs-lookup"><span data-stu-id="38b19-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="38b19-120">คลิกเพื่อเชื่อมต่อ (ปุ่มเปลี่ยนเป็นสีขาว) และคลิก**ส่งทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="38b19-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="38b19-121">**เปิดใช้งานการส่งทันทีเมื่อเชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="38b19-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="38b19-122">บนแท็บ ไฟล์ ให้คลิก**ตัวเลือก**</span><span class="sxs-lookup"><span data-stu-id="38b19-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="38b19-123">ในกล่องโต้ตอบ ตัวเลือก Outlook ให้คลิก**ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="38b19-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="38b19-124">ในส่วน ส่งและรับ ให้คลิก เพื่อเปิดใช้งาน**การส่ง ทันทีเมื่อเชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="38b19-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="38b19-125">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="38b19-125">Click **OK**.</span></span>
 
<span data-ttu-id="38b19-126">สําหรับรายละเอียดทั้งหมด, ดู:</span><span class="sxs-lookup"><span data-stu-id="38b19-126">For full details, see:</span></span>
- [<span data-ttu-id="38b19-127">วิดีโอ: ส่งหรือลบอีเมลที่ค้างอยู่</span><span class="sxs-lookup"><span data-stu-id="38b19-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="38b19-128">อีเมลจะอยู่ในโฟลเดอร์กล่องขาออกจนกว่าคุณจะเริ่มการดําเนินการส่ง/รับใน Outlook ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="38b19-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
