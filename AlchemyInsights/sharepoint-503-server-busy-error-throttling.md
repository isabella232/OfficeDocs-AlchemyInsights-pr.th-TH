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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559860"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5f988-102">ควบคุมปริมาณออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="5f988-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5f988-103">ผู้ใช้อาจได้รับ 503 เซิร์ฟเวอร์ไม่ว่างผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ SharePoint หรือ OneDrive ได้</span><span class="sxs-lookup"><span data-stu-id="5f988-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5f988-104">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="5f988-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5f988-105">ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="5f988-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5f988-106">ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร</span><span class="sxs-lookup"><span data-stu-id="5f988-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5f988-107">ถ้าได้รับควบคุมปริมาณคุณ 99% ของเวลาดังกล่าวจะ มีโค้ดแบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="5f988-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="5f988-108">สำหรับข้อมูลเพิ่มเติมในการควบคุมปริมาณให้ดู[Avoid การควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="5f988-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5f988-109">ถ้าคุณเชื่อว่า ข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ คุณสามารถตรวจสอบถ้าไม่มีการบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="5f988-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5f988-110">ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า[ความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="5f988-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

