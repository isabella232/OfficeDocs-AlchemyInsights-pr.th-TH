---
title: ไม่สามารถเริ่มต้นเวิร์กโฟลว์
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270799"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="bbf2e-102">ไม่สามารถเริ่มต้นเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="bbf2e-102">Workflow is not starting</span></span>

- <span data-ttu-id="bbf2e-103">ลำดับงาน SharePoint 2010 และ SharePoint 2013 จะไม่เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="bbf2e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="bbf2e-104">ถ้าไม่สามารถเริ่มต้นเวิร์กโฟลว์ของคุณ อาจมีปัญหากับบริการชั่วคราวซึ่งผู้ใช้อาจพบความล่าช้าเป็นระยะ ๆ ด้วยความคืบหน้าของลำดับงาน</span><span class="sxs-lookup"><span data-stu-id="bbf2e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="bbf2e-105">ตรวจสอบ[ความสมบูรณ์ของแดชบอร์ดบริการซึ่ง](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เมื่อต้องการดูถ้าองค์กรของคุณได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="bbf2e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="bbf2e-106">ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน</span><span class="sxs-lookup"><span data-stu-id="bbf2e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bbf2e-107">ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน</span><span class="sxs-lookup"><span data-stu-id="bbf2e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bbf2e-108">โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="bbf2e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="bbf2e-109">เวิร์กโฟลว์ SharePoint 2010 ล่าช้าในการเริ่มต้นเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="bbf2e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="bbf2e-110">เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์จะถูกทริกเกอร์เป็นชุดงานขนาดใหญ่</span><span class="sxs-lookup"><span data-stu-id="bbf2e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="bbf2e-111">(ตัวอย่างเช่น เมื่อหลายรายการบวกในคราวเดียวกัน)</span><span class="sxs-lookup"><span data-stu-id="bbf2e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="bbf2e-112">เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อทำงานแบบเรียลไทม์ ดังนั้นการเลื่อนเวลาเป็นลักษณะการทำงานด้วยการออกแบบ</span><span class="sxs-lookup"><span data-stu-id="bbf2e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="bbf2e-113">ถ้าเวิร์กโฟลว์ ซับซ้อน Extensible วัตถุมาร์กอัปภาษา (XMOL), คอมไพล์สามารถทำได้ล่าช้า</span><span class="sxs-lookup"><span data-stu-id="bbf2e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="bbf2e-114">ตรวจสอบบทความ[นี้](https://support.microsoft.com/en-us/kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="bbf2e-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="bbf2e-115">คุณควรทำเวิร์กโฟลว์ หรือออกแบบโดยใช้ชนิดของแพลตฟอร์มเวิร์กโฟลว์ 2013 ของ Microsoft SharePoint</span><span class="sxs-lookup"><span data-stu-id="bbf2e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="bbf2e-116">ถ้าประวัติเวิร์กโฟลว์ของคุณขยายใหญ่จน คุณอาจต้องการกำจัดสินค้า หรือสร้างรายการประวัติใหม่</span><span class="sxs-lookup"><span data-stu-id="bbf2e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="bbf2e-117">หากต้องการข้อมูลเพิ่มเติม:[ล้างประวัติลำดับงาน](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="bbf2e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="bbf2e-118">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="bbf2e-118">Related topics</span></span>
<span data-ttu-id="bbf2e-119">ต้องการลองกระแส Microsoft ใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="bbf2e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="bbf2e-120">สร้างขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="bbf2e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="bbf2e-121">SharePoint และขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="bbf2e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


