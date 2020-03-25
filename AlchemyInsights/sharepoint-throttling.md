---
title: การควบคุมปริมาณแบบออนไลน์ของ SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931461"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ffc41-102">การควบคุมปริมาณแบบออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="ffc41-102">SharePoint Online throttling</span></span>

<span data-ttu-id="ffc41-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="ffc41-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ffc41-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="ffc41-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ffc41-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="ffc41-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ffc41-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="ffc41-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ffc41-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="ffc41-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ffc41-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="ffc41-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ffc41-109">**การควบคุมปริมาณแบบออนไลน์ของ SharePoint**</span><span class="sxs-lookup"><span data-stu-id="ffc41-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="ffc41-110">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ffc41-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ffc41-111">การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="ffc41-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="ffc41-112">สําหรับข้อมูลเพิ่มเติมโปรดไปที่ลิงค์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="ffc41-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="ffc41-113">หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ffc41-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="ffc41-114">การย้ายข้อมูลและการควบคุมปริมาณ SPO</span><span class="sxs-lookup"><span data-stu-id="ffc41-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="ffc41-115">ออนไลน์และ OneDrive ความเร็วในการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="ffc41-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="ffc41-116">จัดการการควบคุมปริมาณ SharePoint แบบออนไลน์ โดยใช้กลับชี้แจงออก</span><span class="sxs-lookup"><span data-stu-id="ffc41-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="ffc41-117">การวางแผนกําลังการผลิตและการทดสอบโหลด SharePoint ออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ffc41-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

