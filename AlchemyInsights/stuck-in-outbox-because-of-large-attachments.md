---
title: ติดอยู่ในกล่องขาออกเนื่องจากมีสิ่งที่แนบมาขนาดใหญ่
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441324"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="01a65-102">แก้ไขข้อความที่ติดอยู่ในกล่องขาออก</span><span class="sxs-lookup"><span data-stu-id="01a65-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="01a65-103">เราขอแนะนำให้คุณเริ่มต้นโดยการเรียกใช้สถานการณ์สมมติ["ฉันมีปัญหาในการส่งการรับหรือการค้นหาข้อความทางเมล"](https://aka.ms/SaRA-OutlookSendReceive)จาก[ฝ่ายสนับสนุนของ Microsoft และเครื่องมือผู้ช่วยกู้คืน](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="01a65-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="01a65-104">เมื่อข้อความได้รับการติดอยู่ในกล่องขาออกของคุณสาเหตุที่มีแนวโน้มมากที่สุดคือ:</span><span class="sxs-lookup"><span data-stu-id="01a65-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="01a65-105">สิ่งที่แนบมาขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="01a65-105">Large attachments.</span></span>
- <span data-ttu-id="01a65-106">การ**ส่งทันทีเมื่อ**ไม่ได้เปิดใช้งานตัวเลือกการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="01a65-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="01a65-107">หากต้องการลบไฟล์แนบขนาดใหญ่:</span><span class="sxs-lookup"><span data-stu-id="01a65-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="01a65-108">ใน Outlook ให้เลือก**ส่ง/รับ** > **งานแบบออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="01a65-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="01a65-109">ในบานหน้าต่างนำทางให้เลือก**กล่องขา**ออก</span><span class="sxs-lookup"><span data-stu-id="01a65-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="01a65-110">จากที่นี่คุณสามารถ:</span><span class="sxs-lookup"><span data-stu-id="01a65-110">From here, you can:</span></span> 
    - <span data-ttu-id="01a65-111">ลบข้อความ (เลือกจากนั้นเลือก**ลบ**)</span><span class="sxs-lookup"><span data-stu-id="01a65-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="01a65-112">ลากข้อความไปยังโฟลเดอร์แบบร่างของคุณคลิกสองครั้งเพื่อเปิดและลบสิ่งที่แนบมาแล้วเลือก**ลบ**)</span><span class="sxs-lookup"><span data-stu-id="01a65-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="01a65-113">ถ้าคุณได้รับข้อผิดพลาดที่ระบุว่า Outlook กำลังพยายามส่งข้อความให้ปิด Outlook</span><span class="sxs-lookup"><span data-stu-id="01a65-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="01a65-114">อาจใช้เวลาสักครู่เพื่อออกจากงาน</span><span class="sxs-lookup"><span data-stu-id="01a65-114">It may take a few moments to exit.</span></span> <span data-ttu-id="01a65-115">ถ้า Outlook ไม่ปิดให้กด Ctrl + Alt + Delete และเลือก**เริ่มต้นตัวจัดการงาน**</span><span class="sxs-lookup"><span data-stu-id="01a65-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="01a65-116">ในตัวจัดการงานให้เลือกแท็บ**กระบวนการ**เลื่อนลงไปที่ outlook .exe และเลือก**กระบวนการสิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="01a65-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="01a65-117">หลังจากที่ Outlook ปิดเริ่มต้นใหม่และทำซ้ำขั้นตอนที่2และ3</span><span class="sxs-lookup"><span data-stu-id="01a65-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="01a65-118">หลังจากที่คุณเอาสิ่งที่แนบมาออกแล้วให้คลิ**กส่ง/รับ** > **งานแบบออฟไลน์**เพื่อดำเนินการทำงานแบบออนไลน์ต่อ</span><span class="sxs-lookup"><span data-stu-id="01a65-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="01a65-119">ข้อความยังได้รับการติดอยู่ในกล่องขาออกเมื่อคุณคลิ**กส่ง**แต่คุณไม่ได้เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="01a65-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="01a65-120">คลิ**กส่ง/รับ**และดูที่ปุ่ม**ทำงานแบบออฟไลน์**</span><span class="sxs-lookup"><span data-stu-id="01a65-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="01a65-121">หากเป็นสีน้ำเงินคุณจะยกเลิกการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="01a65-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="01a65-122">เลือกเพื่อเชื่อมต่อ (ปุ่มเปลี่ยนเป็นสีขาว) และคลิ**กส่งทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="01a65-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="01a65-123">หากต้องการเปิดใช้งานการ**ส่งทันทีเมื่อเชื่อมต่อ**:</span><span class="sxs-lookup"><span data-stu-id="01a65-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="01a65-124">เลือก**ไฟล์** > **ตัวเลือก** >  **ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="01a65-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="01a65-125">ในส่วนของการ**ส่งและรับ**ให้เลือก**ส่งทันทีเมื่อเชื่อมต่อ**แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="01a65-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="01a65-126">สำหรับรายละเอียดทั้งหมดดู:</span><span class="sxs-lookup"><span data-stu-id="01a65-126">For full details see:</span></span>
- [<span data-ttu-id="01a65-127">วิดีโอ: ส่งหรือลบ email ที่ติดอยู่</span><span class="sxs-lookup"><span data-stu-id="01a65-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="01a65-128">เมลจะอยู่ในโฟลเดอร์กล่องขาออกจนกว่าคุณจะเริ่มต้นการดำเนินการส่ง/รับใน Outlook ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="01a65-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
