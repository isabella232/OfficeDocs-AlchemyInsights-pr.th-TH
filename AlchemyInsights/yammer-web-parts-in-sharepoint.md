---
title: Web part ของ Yammer ใน SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664369"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="9d210-102">Web part ของ Yammer ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="9d210-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="9d210-103">การสนทนา yammer และ Yammer ไฮไลต์ web part เพิ่มประสิทธิภาพการทำงานร่วมกันบนหน้า SharePoint ที่ทันสมัยและคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="9d210-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="9d210-104">สำหรับข้อมูลเพิ่มเติมให้ดูที่[การสนทนา yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)และ[ไฮไลต์ของ yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)</span><span class="sxs-lookup"><span data-stu-id="9d210-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="9d210-105">Web part การสนทนา Yammer ที่ทันสมัยกำลังอัปเดตเป็นประสบการณ์การใช้งาน Yammer ใหม่และพร้อมใช้งานสำหรับผู้เช่าที่มีการวางเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="9d210-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="9d210-106">GA ไวร์ได้เริ่มต้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="9d210-106">GA rollout has started.</span></span> <span data-ttu-id="9d210-107">ฟีเจอร์ใหม่รวมถึงความสามารถในการเริ่มต้นการสนทนากับโพสต์ใดๆ (คำถาม, การสำรวจ, การสรรเสริญ) และทำเครื่องหมายคำตอบที่ดีที่สุดโดยตรงจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="9d210-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="9d210-108">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ข้อกำหนดและคำถามที่ถามบ่อยของลูกค้า Yammer ใหม่](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)</span><span class="sxs-lookup"><span data-stu-id="9d210-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="9d210-109">เมื่อต้องการทำความเข้าใจเกี่ยวกับ web part และการกำหนดค่าที่เหมาะกับคุณให้ดูที่การ[ใช้ web part สำหรับ Yammer ใน SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)</span><span class="sxs-lookup"><span data-stu-id="9d210-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="9d210-110">**การใช้ web part กับ SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="9d210-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="9d210-111">Web part สามารถใช้ได้ในหน้าสมัยใหม่และคลาสสิกภายในสภาพแวดล้อมภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="9d210-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="9d210-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับหน้าสมัยใหม่ให้ดู[ที่เพิ่มตัวดึงข้อมูล Yammer ลงในหน้าใหม่ใน SharePoint Server ๒๐๑๙](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019)</span><span class="sxs-lookup"><span data-stu-id="9d210-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="9d210-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับหน้าคลาสสิกให้ดู[ที่เพิ่มตัวดึงข้อมูล Yammer ลงในหน้าคลาสสิกใน SharePoint server ๒๐๑๓, ๒๐๑๖และ๒๐๑๙](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)</span><span class="sxs-lookup"><span data-stu-id="9d210-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="9d210-114">**ฝัง Yammer**</span><span class="sxs-lookup"><span data-stu-id="9d210-114">**Yammer Embed**</span></span>  

<span data-ttu-id="9d210-115">ใช้เครื่องมือการกำหนดค่าฝังเพื่อทดสอบการใช้งานฝัง</span><span class="sxs-lookup"><span data-stu-id="9d210-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="9d210-116">การอัปเดตในอนาคตเพื่อฝังจะเปิดใช้งานประสบการณ์การใช้งาน Yammer ใหม่</span><span class="sxs-lookup"><span data-stu-id="9d210-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="9d210-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [เครื่องมือการกำหนดค่าฝัง](https://aka.ms/YammerEmbedConfigureTool)ตัวของ Yammer</span><span class="sxs-lookup"><span data-stu-id="9d210-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="9d210-118">เมื่อต้องการทำความเข้าใจเกี่ยวกับคอมโพเนนต์ฝังตัวของ Yammer ให้ดูที่[ฝังตัวดึงข้อมูล](https://aka.ms/YammerDevDocs)</span><span class="sxs-lookup"><span data-stu-id="9d210-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="9d210-119">**ปัญหาที่ทราบและข้อจำกัด**</span><span class="sxs-lookup"><span data-stu-id="9d210-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="9d210-120">รหัสกลุ่มจะไม่พร้อมใช้งานจาก Url Yammer ใหม่ซึ่งมีการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="9d210-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="9d210-121">สลับกลับไปยังโหมดคลาสสิกเพื่อรับ Id ของกลุ่มหรือ Id อื่นๆจาก Url</span><span class="sxs-lookup"><span data-stu-id="9d210-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="9d210-122">โดเมนแบบกำหนดเอง (โต๊ะทำงาน) ไม่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="9d210-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="9d210-123">Yammer ฝังตัวไม่ได้รับการปรับให้เหมาะสมสำหรับอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="9d210-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="9d210-124">ใช้หน้าสมัยใหม่ที่มี web part สำหรับการสนทนา Yammer สำหรับประสบการณ์การใช้งานที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="9d210-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="9d210-125">ธีมแบบกำหนดเองจะมีผลต่อลักษณะที่ปรากฏและการใช้งาน web part การสนทนา Yammer</span><span class="sxs-lookup"><span data-stu-id="9d210-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="9d210-126">เปิดกรณีสนับสนุนเพื่อรายงานปัญหา</span><span class="sxs-lookup"><span data-stu-id="9d210-126">Open a support case to report issues.</span></span>