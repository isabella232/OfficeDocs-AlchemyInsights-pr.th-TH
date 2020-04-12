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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232649"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="02518-102">แก้ไขข้อความที่ติดอยู่ในกล่องขาออก</span><span class="sxs-lookup"><span data-stu-id="02518-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="02518-103">เราขอแนะนําให้ คุณเริ่มการทํางาน โดยการเรียกใช้สถานการณ์สมมติ["ฉันมีปัญหาในการส่ง รับ หรือค้นหาข้อความอีเมล"](https://aka.ms/SaRA-OutlookSendReceive)จากเครื่องมือ[สนับสนุนการสนับสนุนและการกู้คืน](https://diagnostics.office.com/#/)ของ Microsoft บนเครื่องที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="02518-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="02518-104">เมื่อข้อความถูกติดอยู่ในกล่องจดหมายออกของคุณ</span><span class="sxs-lookup"><span data-stu-id="02518-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="02518-105">**เอาสิ่งที่แนบมาขนาดใหญ่ออก**</span><span class="sxs-lookup"><span data-stu-id="02518-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="02518-106">คลิก**ส่ง/รับ** > **งานออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="02518-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="02518-107">ในบานหน้าต่างนําทาง ให้คลิก**กล่องขาออก**</span><span class="sxs-lookup"><span data-stu-id="02518-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="02518-108">จากที่นี่ คุณสามารถ:</span><span class="sxs-lookup"><span data-stu-id="02518-108">From here, you can:</span></span> 
    - <span data-ttu-id="02518-109">ลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="02518-109">Delete the message.</span></span> <span data-ttu-id="02518-110">เพียงเลือกและคลิก**ลบ**</span><span class="sxs-lookup"><span data-stu-id="02518-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="02518-111">ลากข้อความไปยังโฟลเดอร์**แบบร่าง**ของคุณ**Delete**</span><span class="sxs-lookup"><span data-stu-id="02518-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="02518-112">ถ้าข้อผิดพลาดแจ้งว่า Outlook กําลังพยายามส่งข้อความ ให้ปิด Outlook</span><span class="sxs-lookup"><span data-stu-id="02518-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="02518-113">มันอาจใช้เวลาสักครู่เพื่อออกจาก</span><span class="sxs-lookup"><span data-stu-id="02518-113">It may take a few moments to exit.</span></span> <span data-ttu-id="02518-114">ถ้า Outlook ไม่ปิด ให้กด**Ctrl+ Alt + Delete**และคลิก**เริ่มตัวจัดการงาน**</span><span class="sxs-lookup"><span data-stu-id="02518-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="02518-115">ใน ตัวจัดการงาน ให้เลือกแท็บ**กระบวนการ**เลื่อนลงไปที่ outlook.exe และคลิก**สิ้นสุดกระบวนการ**</span><span class="sxs-lookup"><span data-stu-id="02518-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="02518-116">หลังจาก Outlook ปิดแล้ว ให้เริ่ม Outlook ใหม่ และทําซ้ําขั้นตอนที่ 2-3</span><span class="sxs-lookup"><span data-stu-id="02518-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="02518-117">หลังจากที่คุณเอาสิ่งที่แนบมาออก ให้คลิก**ส่ง /** > **รับงานแบบออฟไลน์**เพื่อยกเลิกการเลือกปุ่ม และทํางานแบบออนไลน์ต่อ</span><span class="sxs-lookup"><span data-stu-id="02518-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="02518-118">ข้อความยังติดอยู่ในกล่องขาออกเมื่อคุณคลิก**ส่ง**แต่คุณไม่ได้เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="02518-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="02518-119">คลิก**ส่ง / รับ**และดูที่ ปุ่ม**ทํางานแบบออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="02518-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="02518-120">ถ้าเป็นสีน้ําเงิน</span><span class="sxs-lookup"><span data-stu-id="02518-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="02518-121">คลิกเพื่อเชื่อมต่อ (ปุ่มเปลี่ยนเป็นสีขาว) และคลิก**ส่งทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="02518-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="02518-122">**เปิดใช้งานการส่งทันทีเมื่อเชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="02518-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="02518-123">บนแท็บ ไฟล์ ให้คลิก**ตัวเลือก**</span><span class="sxs-lookup"><span data-stu-id="02518-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="02518-124">ในกล่องโต้ตอบ ตัวเลือก Outlook ให้คลิก**ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="02518-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="02518-125">ในส่วน ส่งและรับ ให้คลิก เพื่อเปิดใช้งาน**การส่ง ทันทีเมื่อเชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="02518-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="02518-126">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="02518-126">Click **OK**.</span></span>
 
<span data-ttu-id="02518-127">สําหรับรายละเอียดทั้งหมด, ดู:</span><span class="sxs-lookup"><span data-stu-id="02518-127">For full details, see:</span></span>
- [<span data-ttu-id="02518-128">วิดีโอ: ส่งหรือลบอีเมลที่ค้างอยู่</span><span class="sxs-lookup"><span data-stu-id="02518-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="02518-129">อีเมลจะอยู่ในโฟลเดอร์กล่องขาออกจนกว่าคุณจะเริ่มการดําเนินการส่ง/รับใน Outlook ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="02518-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
