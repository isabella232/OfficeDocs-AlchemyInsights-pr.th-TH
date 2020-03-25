---
title: โยกย้ายตัวเลือกไปยัง SharePoint แบบออนไลน์
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932749"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="4d81d-102">โยกย้ายตัวเลือกไปยัง SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="4d81d-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="4d81d-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="4d81d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4d81d-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4d81d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4d81d-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="4d81d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4d81d-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="4d81d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4d81d-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="4d81d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4d81d-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="4d81d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4d81d-109">**ตัวเลือกการโยกย้าย**</span><span class="sxs-lookup"><span data-stu-id="4d81d-109">**Migration options**</span></span>

<span data-ttu-id="4d81d-110">มีตัวเลือกต่างๆ ที่จะโยกย้ายเนื้อหาไปยัง SharePoint Online ขึ้นอยู่กับขนาดและปริมาณของไฟล์ที่คุณต้องการย้าย โปรดดูรายการของตัวเลือก[ที่อยู่ที่นี่](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="4d81d-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="4d81d-111">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการย้ายข้อมูลเนื้อหา โปรดไปที่ลิงก์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="4d81d-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="4d81d-112">เครื่องมือการโยกย้าย SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d81d-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="4d81d-113">เริ่มต้นใช้งานตัวจัดการการย้าย</span><span class="sxs-lookup"><span data-stu-id="4d81d-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="4d81d-114">ความเร็วการโยกย้ายของ Sharepoint แบบออนไลน์และ ODB</span><span class="sxs-lookup"><span data-stu-id="4d81d-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="4d81d-115">หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="4d81d-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="4d81d-116">เครื่องมือการประเมินการโยกย้าย SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="4d81d-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="4d81d-117">**หมายเหตุ**: ขณะนี้เครื่องมือการโยกย้าย SharePoint สนับสนุนการย้ายจาก SharePoint 2010 และ 2013 เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="4d81d-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="4d81d-118">เวอร์ชัน 2016 หรือ 2019 ไม่ได้รับการสนับสนุนในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="4d81d-118">Version 2016 or 2019 are not supported at this time.</span></span>
