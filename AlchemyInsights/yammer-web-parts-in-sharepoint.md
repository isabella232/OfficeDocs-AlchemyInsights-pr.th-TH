---
title: Web Part Yammer ใน SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198384"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="253a1-102">Web Part Yammer ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="253a1-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="253a1-103">การสนทนา Yammer และ Yammer เน้น Web Part ช่วยเพิ่มการทํางานร่วมกันบนเพจ SharePoint สมัยใหม่และแบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="253a1-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="253a1-104">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การสนทนา Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)และ[ไฮไลต์ของ Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)</span><span class="sxs-lookup"><span data-stu-id="253a1-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="253a1-105">Web Part การสนทนา Yammer สมัยใหม่กําลังถูกปรับปรุงให้ประสบการณ์ใช้งาน Yammer ใหม่ และพร้อมใช้งานสําหรับผู้เช่าที่นําออกใช้เป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="253a1-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="253a1-106">เปิดตัว GA ได้เริ่มต้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="253a1-106">GA rollout has started.</span></span> <span data-ttu-id="253a1-107">คุณลักษณะใหม่รวมถึงความสามารถในการเริ่มต้นการสนทนากับโพสต์ใด ๆ (คําถาม, โพลล์, สรรเสริญ) และทําเครื่องหมายคําตอบที่ดีที่สุดโดยตรงจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="253a1-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="253a1-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ข้อกําหนดของลูกค้าและคําถามที่ถามบ่อยเกี่ยวกับ Yammer ใหม่](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)</span><span class="sxs-lookup"><span data-stu-id="253a1-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="253a1-109">เมื่อต้องการทําความเข้าใจว่า Web Part และการกําหนดค่าใดเหมาะกับคุณ ให้ดูที่[ใช้ Web Part Yammer ใน SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)</span><span class="sxs-lookup"><span data-stu-id="253a1-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="253a1-110">**การใช้ Web Part กับเซิร์ฟเวอร์ SharePoint**</span><span class="sxs-lookup"><span data-stu-id="253a1-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="253a1-111">Web Part สามารถใช้ในเพจสมัยใหม่และคลาสสิกภายในสภาพแวดล้อมในสถานที่</span><span class="sxs-lookup"><span data-stu-id="253a1-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="253a1-112">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเพจสมัยใหม่ ให้ดูที่[การเพิ่มตัวดึงข้อมูล Yammer ไปยังเพจสมัยใหม่ใน SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019)</span><span class="sxs-lookup"><span data-stu-id="253a1-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="253a1-113">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเพจแบบคลาสสิก ให้ดูที่[การเพิ่มตัวดึงข้อมูล Yammer ไปยังเพจแบบคลาสสิคใน SharePoint Servers 2013, 2016 และ 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)</span><span class="sxs-lookup"><span data-stu-id="253a1-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="253a1-114">**ฝัง Yammer**</span><span class="sxs-lookup"><span data-stu-id="253a1-114">**Yammer Embed**</span></span>  

<span data-ttu-id="253a1-115">ใช้เครื่องมือการกําหนดค่าฝังเพื่อทดสอบการใช้งานฝัง</span><span class="sxs-lookup"><span data-stu-id="253a1-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="253a1-116">การปรับปรุงในอนาคตเพื่อฝังจะเปิดใช้งานประสบการณ์การใช้งาน Yammer ใหม่</span><span class="sxs-lookup"><span data-stu-id="253a1-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="253a1-117">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[เครื่องมือการกําหนดค่าการฝัง Yammer](https://aka.ms/YammerEmbedConfigureTool)</span><span class="sxs-lookup"><span data-stu-id="253a1-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="253a1-118">เมื่อต้องการทําความเข้าใจคอมโพเนนต์ Yammer Embed ให้ดียิ่งขึ้น ให้ดูที่[ฝังตัวดึงข้อมูล](https://aka.ms/YammerDevDocs)</span><span class="sxs-lookup"><span data-stu-id="253a1-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="253a1-119">**ปัญหาที่ทราบและข้อจํากัด**</span><span class="sxs-lookup"><span data-stu-id="253a1-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="253a1-120">ID กลุ่มไม่พร้อมใช้งานจาก Url Yammer ใหม่ ซึ่งมีการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="253a1-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="253a1-121">สลับกลับไปยังโหมดคลาสสิกเพื่อรับข้อมูลกลุ่มหรือไอดีอื่นจาก URL</span><span class="sxs-lookup"><span data-stu-id="253a1-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="253a1-122">ไม่สนับสนุนโดเมนแบบกําหนดเอง (vanity)</span><span class="sxs-lookup"><span data-stu-id="253a1-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="253a1-123">Yammer ฝังไม่ได้รับการปรับให้เหมาะสมสําหรับอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="253a1-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="253a1-124">ใช้เพจสมัยใหม่กับ Web Part การสนทนา Yammer เพื่อประสบการณ์ที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="253a1-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="253a1-125">ชุดรูปแบบแบบกําหนดเองอาจมีผลต่อลักษณะที่ปรากฏและการใช้งานของ Web Part การสนทนา Yammer</span><span class="sxs-lookup"><span data-stu-id="253a1-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="253a1-126">เปิดกรณีสนับสนุนเพื่อรายงานปัญหา</span><span class="sxs-lookup"><span data-stu-id="253a1-126">Open a support case to report issues.</span></span>