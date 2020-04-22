---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766116"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="2fef4-102">เวิร์กโฟลว์ไม่ได้เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="2fef4-102">Workflow is not starting</span></span>

- <span data-ttu-id="2fef4-103">เวิร์กโฟลว์ SharePoint 2010 และ SharePoint 2013 จะไม่เริ่มทํางาน</span><span class="sxs-lookup"><span data-stu-id="2fef4-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="2fef4-104">ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มต้น อาจมีปัญหาการบริการชั่วคราวซึ่งผู้ใช้อาจพบความล่าช้าเป็นระยะ ๆ กับความคืบหน้าของเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="2fef4-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="2fef4-105">ตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="2fef4-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="2fef4-106">หากผ่านเกิน 24 ชั่วโมงตั้งแต่เห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="2fef4-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2fef4-107">ในหลายกรณีเรากําลังทํางานเกี่ยวกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="2fef4-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2fef4-108">โปรดให้เราอย่างน้อย 24 ชั่วโมงเพื่อแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="2fef4-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="2fef4-109">เวิร์กโฟลว์ SharePoint 2010 ล่าช้าเมื่อเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="2fef4-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="2fef4-110">เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์จะถูกทริกเกอร์ในชุดงานขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="2fef4-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="2fef4-111">(ตัวอย่างเช่น เมื่อมีหลายรายการถูกเพิ่มในครั้งเดียว)</span><span class="sxs-lookup"><span data-stu-id="2fef4-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="2fef4-112">เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อทํางานแบบเรียลไทม์ ดังนั้นความล่าช้าคือลักษณะการทํางานการออกแบบ</span><span class="sxs-lookup"><span data-stu-id="2fef4-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="2fef4-113">ถ้ากระแสงานเป็นภาษามาร์กอัปวัตถุ Extensible ซับซ้อน (XMOL), การคอมไพล์สามารถช้า</span><span class="sxs-lookup"><span data-stu-id="2fef4-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="2fef4-114">ตรวจสอบ[บทความนี้](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="2fef4-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="2fef4-115">คุณควรทําให้เวิร์กโฟลว์ง่ายขึ้นหรือออกแบบใหม่โดยใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ของ Microsoft SharePoint 2013</span><span class="sxs-lookup"><span data-stu-id="2fef4-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="2fef4-116">ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้นคุณอาจต้องการล้างรายการหรือสร้างรายการประวัติใหม่</span><span class="sxs-lookup"><span data-stu-id="2fef4-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="2fef4-117">ข้อมูลเพิ่มเติม :[ประวัติเวิร์กโฟลว์การล้างข้อมูล](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="2fef4-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="2fef4-118">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="2fef4-118">Related topics</span></span>
<span data-ttu-id="2fef4-119">ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="2fef4-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2fef4-120">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="2fef4-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2fef4-121">SharePoint และโฟลว์</span><span class="sxs-lookup"><span data-stu-id="2fef4-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


