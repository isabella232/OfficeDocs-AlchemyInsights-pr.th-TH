---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403762"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="288fb-102">เวิร์กโฟลว์ไม่ได้เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="288fb-102">Workflow is not starting</span></span>

- <span data-ttu-id="288fb-103">เวิร์กโฟลว์ SharePoint 2010 และ SharePoint 2013 ไม่เริ่มขึ้น</span><span class="sxs-lookup"><span data-stu-id="288fb-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="288fb-104">ถ้าเวิร์กโฟลว์ของคุณไม่เริ่มขึ้น อาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้อาจพบความล่าช้าในความคืบหน้าของเวิร์กโฟลว์เป็นระยะๆ</span><span class="sxs-lookup"><span data-stu-id="288fb-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="288fb-105">ตรวจสอบ [แดชบอร์ดสถาน](https://admin.microsoft.com/AdminPortal/Home/servicehealth) ภาพบริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="288fb-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="288fb-106">หากเวลาผ่านไปมากกว่า 24 ชั่วโมงหลังจากที่คุณเห็นปัญหานี้เป็นครั้งแรก โปรดบันทึกตั๋วการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="288fb-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="288fb-107">ในหลายกรณี เราหาวิธีแก้ไขแล้ว</span><span class="sxs-lookup"><span data-stu-id="288fb-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="288fb-108">โปรดให้เวลาเราอย่างน้อย 24 ชั่วโมงเพื่อแก้ไขปัญหาให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="288fb-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="288fb-109">เวิร์กโฟลว์ SharePoint 2010 หน่วงเวลาเมื่อเริ่มใช้งาน</span><span class="sxs-lookup"><span data-stu-id="288fb-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="288fb-110">ซึ่งจะเกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์เป็นชุดใหญ่</span><span class="sxs-lookup"><span data-stu-id="288fb-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="288fb-111">(ตัวอย่างเช่น เมื่อมีการเพิ่มหลายรายการในครั้งเดียว)</span><span class="sxs-lookup"><span data-stu-id="288fb-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="288fb-112">เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อเรียกใช้แบบเรียลไทม์ ดังนั้นการหน่วงเวลาจึงเกิดขึ้นตามลักษณะการดีไซน์</span><span class="sxs-lookup"><span data-stu-id="288fb-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="288fb-113">ถ้าเวิร์กโฟลว์ซับซ้อน Extensible Object Markup Language (XRUP) การคอมไพล์อาจช้าได้</span><span class="sxs-lookup"><span data-stu-id="288fb-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="288fb-114">[ตรวจสอบ](https://support.microsoft.com//kb/3043697)บทความนี้</span><span class="sxs-lookup"><span data-stu-id="288fb-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="288fb-115">คุณควรลดความซับซ้อนของเวิร์กโฟลว์หรือออกแบบใหม่โดยใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ของ Microsoft SharePoint 2013</span><span class="sxs-lookup"><span data-stu-id="288fb-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="288fb-116">ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้น คุณอาจต้องการล้างข้อมูลหรือสร้างรายการประวัติใหม่</span><span class="sxs-lookup"><span data-stu-id="288fb-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="288fb-117">ข้อมูลเพิ่มเติม : [การล้างประวัติเวิร์กโฟลว์](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="288fb-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="288fb-118">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="288fb-118">Related topics</span></span>
<span data-ttu-id="288fb-119">ต้องการลองใช้ Microsoft Flow ใน SharePoint Online ใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="288fb-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="288fb-120">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="288fb-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="288fb-121">SharePoint และ Flow</span><span class="sxs-lookup"><span data-stu-id="288fb-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
