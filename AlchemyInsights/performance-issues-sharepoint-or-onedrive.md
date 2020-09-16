---
title: ปัญหาด้านประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771920"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="6cb07-102">SharePoint หรือ OneDrive ช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="6cb07-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="6cb07-103">SharePoint หรือ OneDrive อาจทำให้ไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานหรืออาจไม่พร้อมใช้งานหรืออาจแสดงข้อผิดพลาดของบริการที่ไม่พร้อมใช้งานหรือข้อผิดพลาด๕๐๓ด้วยเหตุผลหลายประการดังนี้</span><span class="sxs-lookup"><span data-stu-id="6cb07-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="6cb07-104">ถ้าไซต์ SharePoint หรือ OneDrive ของคุณช้าหรือล่าช้าสำหรับผู้ใช้หลายคนอาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้ประสบปัญหาความล่าช้าหรือข้อผิดพลาดในการนำทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive</span><span class="sxs-lookup"><span data-stu-id="6cb07-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="6cb07-105">ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="6cb07-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="6cb07-106">ผู้ใช้อาจได้รับข้อผิดพลาดที่ *ไม่ว่างของ๕๐๓* เมื่อพยายามนำทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="6cb07-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="6cb07-107">ข้อผิดพลาดนี้อาจมีสาเหตุมาจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6cb07-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6cb07-108">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6cb07-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6cb07-109">การควบคุมปริมาณจะจำกัดจำนวนการดำเนินการของผู้ใช้หรือการโทรที่พร้อมกัน (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้มีทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="6cb07-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6cb07-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณให้ดูที่[หลีกเลี่ยงการปริมาณหรือการบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="6cb07-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="6cb07-111">ถ้าคุณพบประสิทธิภาพการทำงานที่ช้าลงด้วยไซต์หรือไซต์ SharePoint แบบ **คลาสสิก** หรือ **สมัยใหม่** ให้ใช้ [เครื่องมือการวินิจฉัยหน้า](https://aka.ms/perftool) เพื่อวิเคราะห์หน้า</span><span class="sxs-lookup"><span data-stu-id="6cb07-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="6cb07-112">ถ้าคุณยังคงพบประสิทธิภาพการทำงานที่ช้าทั่วไปโปรดตรวจทานทรัพยากรที่ด้านล่างของบทความนี้: [บทนำสู่การปรับปรุงประสิทธิภาพการทำงานสำหรับ SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="6cb07-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  