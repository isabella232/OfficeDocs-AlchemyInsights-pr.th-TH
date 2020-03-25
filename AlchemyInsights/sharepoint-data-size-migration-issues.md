---
title: ปัญหาขณะกําลังโยกย้ายข้อมูลไปยัง SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931713"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="7731a-102">ปัญหาขณะกําลังโยกย้ายข้อมูลไปยัง SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7731a-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="7731a-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="7731a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7731a-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="7731a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7731a-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="7731a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7731a-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="7731a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7731a-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="7731a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7731a-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="7731a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7731a-109">**การโยกย้ายข้อมูลมากกว่า 100TB**</span><span class="sxs-lookup"><span data-stu-id="7731a-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="7731a-110">ดูเหมือนว่าคุณกําลังย้ายข้อมูลมากกว่า 100TB ไปยัง SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7731a-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="7731a-111">โปรดทําตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยคุณโดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="7731a-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="7731a-112">เลือก**คําขอบริการใหม่**แล้วเลือก**คําขอบริการใหม่**</span><span class="sxs-lookup"><span data-stu-id="7731a-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="7731a-113">ปล่อยชื่อเรื่องและคําอธิบายไว้เป็น**การย้าย SharePoint มากกว่า 100TB**</span><span class="sxs-lookup"><span data-stu-id="7731a-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="7731a-114">เมื่อตั๋วถูกส่งไปแล้ว โปรดอัปเดตด้วยข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7731a-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="7731a-115">ขนาดโดยประมาณของการย้ายข้อมูล</span><span class="sxs-lookup"><span data-stu-id="7731a-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="7731a-116">ค่าประมาณของเวลาที่คุณต้องการเริ่มต้นและดําเนินการย้ายให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="7731a-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="7731a-117">อธิบายตําแหน่งที่คุณกําลังย้ายเนื้อหาของคุณ เช่น SharePoint Server, Box, GDrive, การแชร์ไฟล์ และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="7731a-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

