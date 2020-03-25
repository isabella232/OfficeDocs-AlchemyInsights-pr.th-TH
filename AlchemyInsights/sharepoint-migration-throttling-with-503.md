---
title: การควบคุมปริมาณการโยกย้าย SharePoint ที่มีข้อผิดพลาด 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931677"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="c5e4f-102">การควบคุมปริมาณการโยกย้าย SharePoint ที่มีข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="c5e4f-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="c5e4f-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="c5e4f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c5e4f-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="c5e4f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c5e4f-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="c5e4f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c5e4f-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="c5e4f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c5e4f-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="c5e4f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c5e4f-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="c5e4f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c5e4f-109">**ข้อผิดพลาด 503 เมื่อโยกย้ายไปยัง SharePoint แบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="c5e4f-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="c5e4f-110">ดูเหมือนว่าคุณกําลังโยกย้ายไปยัง SharePoint Online และรับข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="c5e4f-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="c5e4f-111">โปรดทําตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยคุณโดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="c5e4f-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="c5e4f-112">คลิก**ติดต่อฝ่ายสนับสนุน**แล้วคลิก**คําขอบริการใหม่**</span><span class="sxs-lookup"><span data-stu-id="c5e4f-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="c5e4f-113">สําหรับชื่อเรื่องและคําอธิบาย ให้พิมพ์**การควบคุมปริมาณการย้าย SharePoint ด้วย 503**</span><span class="sxs-lookup"><span data-stu-id="c5e4f-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="c5e4f-114">เมื่อตั๋วถูกส่งไปแล้ว โปรดอัปเดตด้วยข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c5e4f-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="c5e4f-115">จํานวนการโยกย้าย (เช่น จํานวน TBs)</span><span class="sxs-lookup"><span data-stu-id="c5e4f-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="c5e4f-116">วันที่เริ่มต้นและวันที่สิ้นสุดการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="c5e4f-116">Migration start and end date.</span></span>
    - <span data-ttu-id="c5e4f-117">อธิบายตําแหน่งที่คุณกําลังย้ายเนื้อหาของคุณ เช่น SharePoint Server, Box, GDrive, การแชร์ไฟล์ และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="c5e4f-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="c5e4f-118">ประมาณจํานวนข้อผิดพลาดการควบคุมปริมาณ (ตัวอย่างเช่น การควบคุมปริมาณ x ต่อชั่วโมง)และเมื่อการควบคุมปริมาณเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="c5e4f-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="c5e4f-119">เครื่องมือการโยกย้ายที่คุณกําลังใช้ (ตัวอย่างเช่น SPMT หรือ ShareGate)</span><span class="sxs-lookup"><span data-stu-id="c5e4f-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


