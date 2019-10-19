---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738108"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="50ce3-102">เวิร์กโฟลว์ไม่ได้เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="50ce3-102">Workflow is not starting</span></span>

- <span data-ttu-id="50ce3-103">ไม่มีการเริ่มทำงาน SharePoint ๒๐๑๐และ SharePoint ๒๐๑๓เวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="50ce3-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="50ce3-104">ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มต้นอาจมีปัญหาการบริการแบบถาวรที่ผู้ใช้อาจพบความล่าช้าเป็นระยะๆกับความคืบหน้าของเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="50ce3-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="50ce3-105">ตรวจสอบ[แดชบอร์ดความสมบูรณ์ของบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="50ce3-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="50ce3-106">หากมีการผ่านมากกว่า24ชั่วโมงตั้งแต่แรกคุณเห็นปัญหานี้โปรดบันทึกตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="50ce3-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="50ce3-107">ในหลายกรณีเรากำลังทำงานอยู่แล้วในการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="50ce3-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="50ce3-108">กรุณาให้เราอย่างน้อย24ชั่วโมงในการดำเนินการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="50ce3-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="50ce3-109">ลำดับงาน SharePoint ๒๐๑๐ที่ล่าช้าเมื่อเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="50ce3-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="50ce3-110">เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์ในชุดงานขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="50ce3-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="50ce3-111">(ตัวอย่างเช่นเมื่อมีการเพิ่มสินค้าหลายรายการพร้อมกัน)</span><span class="sxs-lookup"><span data-stu-id="50ce3-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="50ce3-112">เวิร์กโฟลว์ไม่ได้รับการออกแบบให้รันแบบเรียลไทม์เพื่อให้การหน่วงเวลาเป็นลักษณะการทำงานออกแบบ</span><span class="sxs-lookup"><span data-stu-id="50ce3-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="50ce3-113">ถ้าเวิร์กโฟลว์เป็นภาษามาร์กอัปวัตถุ Extensible ที่ซับซ้อน (XMOL) การคอมไพล์สามารถทำได้ช้า</span><span class="sxs-lookup"><span data-stu-id="50ce3-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="50ce3-114">ตรวจสอบบทความ[นี้](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="50ce3-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="50ce3-115">คุณควรทำให้เวิร์กโฟลว์ของคุณง่ายขึ้นหรือออกแบบโดยใช้ชนิดแพลตฟอร์มของเวิร์กโฟลว์ Microsoft SharePoint ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="50ce3-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="50ce3-116">ถ้าประวัติลำดับงานของคุณเติบโตขึ้นใหญ่คุณอาจต้องการล้างรายการหรือสร้างรายการประวัติใหม่</span><span class="sxs-lookup"><span data-stu-id="50ce3-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="50ce3-117">ข้อมูลเพิ่มเติม:[ล้างประวัติลำดับงาน](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="50ce3-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="50ce3-118">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="50ce3-118">Related topics</span></span>
<span data-ttu-id="50ce3-119">ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="50ce3-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="50ce3-120">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="50ce3-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="50ce3-121">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="50ce3-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


