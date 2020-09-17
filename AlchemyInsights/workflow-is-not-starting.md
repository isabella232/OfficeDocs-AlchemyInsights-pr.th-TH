---
title: เวิร์กโฟลว์ไม่เริ่มทำงาน
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794786"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="7c8ac-102">เวิร์กโฟลว์ไม่เริ่มทำงาน</span><span class="sxs-lookup"><span data-stu-id="7c8ac-102">Workflow is not starting</span></span>

- <span data-ttu-id="7c8ac-103">เวิร์กโฟลว์ SharePoint ๒๐๑๐และ SharePoint ๒๐๑๓จะไม่เริ่มทำงาน</span><span class="sxs-lookup"><span data-stu-id="7c8ac-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="7c8ac-104">ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มทำงานอาจมีปัญหาในการบริการชั่วคราวที่ผู้ใช้อาจพบความล่าช้าเป็นระยะๆด้วยความคืบหน้าของเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="7c8ac-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="7c8ac-105">ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="7c8ac-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="7c8ac-106">ถ้าคุณได้รับการส่งผ่านมากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="7c8ac-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7c8ac-107">ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="7c8ac-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7c8ac-108">โปรดแจ้งให้เราทราบอย่างน้อย24ชั่วโมงเพื่อให้โซลูชันเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="7c8ac-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="7c8ac-109">เวิร์กโฟลว์ SharePoint ๒๐๑๐ล่าช้าเมื่อเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="7c8ac-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="7c8ac-110">เหตุการณ์นี้จะเกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์ในชุดขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="7c8ac-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="7c8ac-111">(ตัวอย่างเช่นเมื่อมีการเพิ่มรายการหลายรายการในครั้งเดียว)</span><span class="sxs-lookup"><span data-stu-id="7c8ac-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="7c8ac-112">เวิร์กโฟลว์ไม่ได้รับการออกแบบมาให้ทำงานแบบเรียลไทม์ดังนั้นการหน่วงเวลาคือการทำงานโดยการออกแบบ</span><span class="sxs-lookup"><span data-stu-id="7c8ac-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="7c8ac-113">ถ้าเวิร์กโฟลว์เป็นภาษาที่ซับซ้อน Extensible Object Markup Language (XMOL) การคอมไพล์สามารถทำงานได้ช้า</span><span class="sxs-lookup"><span data-stu-id="7c8ac-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="7c8ac-114">ตรวจสอบบทความ[นี้](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="7c8ac-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="7c8ac-115">คุณควรทำให้เวิร์กโฟลว์ทำงานได้ง่ายขึ้นหรือออกแบบใหม่โดยใช้ชนิดของแพลตฟอร์มสำหรับเวิร์กโฟลว์ของ Microsoft SharePoint ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="7c8ac-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="7c8ac-116">ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้นคุณอาจต้องการล้างข้อมูลรายการหรือสร้างรายการประวัติใหม่</span><span class="sxs-lookup"><span data-stu-id="7c8ac-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="7c8ac-117">ข้อมูลเพิ่มเติม: การ [ล้างประวัติของเวิร์กโฟลว์](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="7c8ac-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="7c8ac-118">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="7c8ac-118">Related topics</span></span>
<span data-ttu-id="7c8ac-119">ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่</span><span class="sxs-lookup"><span data-stu-id="7c8ac-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7c8ac-120">สร้างขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="7c8ac-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7c8ac-121">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="7c8ac-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


