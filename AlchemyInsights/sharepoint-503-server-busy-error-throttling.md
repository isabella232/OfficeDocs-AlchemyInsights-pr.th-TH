---
title: การควบคุมปริมาณแบบออนไลน์ของ SharePoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931245"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="4d8f4-102">การควบคุมปริมาณแบบออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d8f4-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="4d8f4-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="4d8f4-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4d8f4-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4d8f4-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4d8f4-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="4d8f4-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4d8f4-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="4d8f4-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4d8f4-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="4d8f4-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4d8f4-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="4d8f4-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4d8f4-109">**ข้อผิดพลาดของเซิร์ฟเวอร์ 503 ไม่ว่าง**</span><span class="sxs-lookup"><span data-stu-id="4d8f4-109">**503 server is busy error**</span></span>

<span data-ttu-id="4d8f4-110">ผู้ใช้อาจได้รับเซิร์ฟเวอร์ 503 ไม่ว่างข้อผิดพลาดเมื่อพยายามที่จะนําทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="4d8f4-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="4d8f4-111">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d8f4-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4d8f4-112">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="4d8f4-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4d8f4-113">การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="4d8f4-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="4d8f4-114">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณ ให้ดูที่[หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="4d8f4-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="4d8f4-115">ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ[Message center](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="4d8f4-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="4d8f4-116">ตรวจสอบคําแนะนํา/เหตุการณ์ที่อาจเกิดขึ้น[Service Health](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="4d8f4-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

