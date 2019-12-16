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
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048635"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1c03e-102">การควบคุมปริมาณแบบออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="1c03e-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1c03e-103">ผู้ใช้อาจได้รับเซิร์ฟเวอร์๕๐๓มีข้อผิดพลาดไม่ว่างเมื่อพยายามนำทางไปยังไซต์ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="1c03e-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1c03e-104">ข้อผิดพลาดนี้อาจเกิดจากการควบคุมปริมาณภายในบริการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="1c03e-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1c03e-105">SharePoint แบบออนไลน์ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพการทำงานที่ดีที่สุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="1c03e-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1c03e-106">การควบคุมปริมาณจะจำกัดจำนวนของการดำเนินการของผู้ใช้หรือการโทรที่เกิดขึ้นพร้อมกัน (โดยใช้สคริปต์หรือรหัส) เพื่อป้องกันไม่ให้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="1c03e-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="1c03e-107">ถ้าคุณได้รับการควบคุมปริมาณ, ๙๙% ของเวลาที่เป็นเพราะรหัสที่กำหนดเอง.</span><span class="sxs-lookup"><span data-stu-id="1c03e-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="1c03e-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการควบคุมปริมาณการใช้งานโปรดหลีกเลี่ยงการใช้งาน[หรือถูกบล็อคใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="1c03e-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1c03e-109">ถ้าคุณเชื่อว่าข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณคุณสามารถตรวจสอบว่ามีการบำรุงรักษาที่ใช้งานอยู่ในผู้เช่าของคุณโดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="1c03e-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1c03e-110">ในที่สุด, ให้แน่ใจว่าคุณเยี่ยมชมหน้า[สุขภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจสอบคำแนะนำใดๆ/เหตุการณ์ที่อาจเกิดขึ้น.</span><span class="sxs-lookup"><span data-stu-id="1c03e-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

