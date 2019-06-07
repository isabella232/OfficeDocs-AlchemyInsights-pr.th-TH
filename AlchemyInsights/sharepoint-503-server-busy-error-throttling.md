---
title: ควบคุมปริมาณออนไลน์ของ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761277"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="9eca8-102">ควบคุมปริมาณออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9eca8-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="9eca8-103">ผู้ใช้อาจได้รับ 503 เซิร์ฟเวอร์ไม่ว่างผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ SharePoint หรือ OneDrive ได้</span><span class="sxs-lookup"><span data-stu-id="9eca8-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="9eca8-104">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9eca8-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9eca8-105">ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9eca8-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9eca8-106">ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร</span><span class="sxs-lookup"><span data-stu-id="9eca8-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="9eca8-107">ถ้าได้รับควบคุมปริมาณคุณ 99% ของเวลาดังกล่าวจะ มีโค้ดแบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="9eca8-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="9eca8-108">สำหรับข้อมูลเพิ่มเติมในการควบคุมปริมาณให้ดู[Avoid การควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="9eca8-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="9eca8-109">ถ้าคุณเชื่อว่า ข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ คุณสามารถตรวจสอบถ้าไม่มีการบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="9eca8-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="9eca8-110">ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า[ความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="9eca8-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

