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
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958754"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="d6f90-102">การควบคุมปริมาณแบบออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="d6f90-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="d6f90-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d6f90-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d6f90-104">**ข้อผิดพลาดของเซิร์ฟเวอร์ 503 ไม่ว่าง**</span><span class="sxs-lookup"><span data-stu-id="d6f90-104">**503 server is busy error**</span></span>

<span data-ttu-id="d6f90-105">ผู้ใช้อาจได้รับเซิร์ฟเวอร์ 503 ไม่ว่างข้อผิดพลาดเมื่อพยายามที่จะนําทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="d6f90-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="d6f90-106">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="d6f90-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="d6f90-107">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d6f90-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d6f90-108">การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="d6f90-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="d6f90-109">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณ ให้ดูที่[หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="d6f90-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="d6f90-110">ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ[Message center](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="d6f90-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="d6f90-111">ตรวจสอบคําแนะนํา/เหตุการณ์ที่อาจเกิดขึ้น[Service Health](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="d6f90-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

