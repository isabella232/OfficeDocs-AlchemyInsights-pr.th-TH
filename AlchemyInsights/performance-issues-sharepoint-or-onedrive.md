---
title: ปัญหาประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068439"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="caba9-102">SharePoint หรือ OneDrive ช้า, ไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="caba9-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="caba9-103">SharePoint หรือ OneDrive อาจทำงานช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานหรืออาจแสดงข้อผิดพลาดของบริการที่ไม่พร้อมใช้งานหรือ๕๐๓ด้วยเหตุผลหลายประการ:</span><span class="sxs-lookup"><span data-stu-id="caba9-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="caba9-104">ถ้าไซต์ SharePoint หรือ OneDrive ของคุณช้าหรือล่าช้าสำหรับผู้ใช้หลายคนอาจมีปัญหาการบริการแบบถาวรที่ผู้ใช้พบความล่าช้าหรือข้อผิดพลาดการนำทางเป็นระยะๆเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive</span><span class="sxs-lookup"><span data-stu-id="caba9-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="caba9-105">ตรวจสอบ[แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="caba9-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="caba9-106">ผู้ใช้อาจได้รับ*๕๐๓เซิร์ฟเวอร์ไม่ว่าง*ข้อผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="caba9-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="caba9-107">ข้อผิดพลาดนี้อาจเกิดจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="caba9-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="caba9-108">SharePoint แบบออนไลน์ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="caba9-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="caba9-109">การควบคุมปริมาณจะจำกัดจำนวนของการดำเนินการของผู้ใช้หรือการโทรที่เกิดขึ้นพร้อมกัน (โดยใช้สคริปต์หรือรหัส) เพื่อป้องกันไม่ให้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="caba9-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="caba9-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณการใช้งานโปรดหลีกเลี่ยงการใช้งาน[หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="caba9-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="caba9-111">ถ้าคุณพบกับประสิทธิภาพการทำงานที่ช้าด้วยไซต์หรือเพจ SharePoint แบบ**คลาสสิก**หรือ**สมัยใหม่**ให้ใช้[เครื่องมือวินิจฉัยหน้า](https://aka.ms/perftool)เพื่อวิเคราะห์เพจ</span><span class="sxs-lookup"><span data-stu-id="caba9-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="caba9-112">หากคุณยังคงพบประสิทธิภาพการทำงานช้าทั่วไปโปรดตรวจทานทรัพยากรที่ด้านล่างของบทความนี้:[บทนำเกี่ยวกับการปรับประสิทธิภาพการทำงานสำหรับ SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="caba9-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  