---
title: การควบคุมปริมาณ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773866"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="9bd7b-102">การควบคุมปริมาณ SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9bd7b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="9bd7b-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="9bd7b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9bd7b-104">**เซิร์ฟเวอร์๕๐๓มีข้อผิดพลาดที่ไม่ว่าง**</span><span class="sxs-lookup"><span data-stu-id="9bd7b-104">**503 server is busy error**</span></span>

<span data-ttu-id="9bd7b-105">ผู้ใช้อาจได้รับข้อผิดพลาดที่ไม่ว่างของ๕๐๓เมื่อพยายามนำทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9bd7b-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="9bd7b-106">ข้อผิดพลาดนี้อาจมีสาเหตุมาจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9bd7b-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9bd7b-107">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9bd7b-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9bd7b-108">การควบคุมปริมาณจะจำกัดจำนวนการดำเนินการของผู้ใช้หรือการโทรที่พร้อมกัน (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้มีทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="9bd7b-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="9bd7b-109">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณให้ดูที่[หลีกเลี่ยงการปริมาณหรือการบล็อกใน SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="9bd7b-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="9bd7b-110">ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณคุณสามารถตรวจสอบว่ามีการบำรุงรักษาที่ใช้งานอยู่ในผู้เช่าของคุณหรือไม่โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="9bd7b-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="9bd7b-111">สุดท้ายให้ตรวจสอบให้แน่ใจว่าคุณได้เยี่ยมชมหน้า [สถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth) เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="9bd7b-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

