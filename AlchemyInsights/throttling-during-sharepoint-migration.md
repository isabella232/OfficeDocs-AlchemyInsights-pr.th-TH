---
title: การควบคุมปริมาณในระหว่างการโยกย้าย SharePoint
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1987"
- "9000353"
ms.assetid: ''
ms.openlocfilehash: c42f9a274edf3a5617ca8d05aa7a4ea3ef18a8db
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353952"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="0e8d6-102">การควบคุมปริมาณของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e8d6-102">SharePoint throttling</span></span>

<span data-ttu-id="0e8d6-103">ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e8d6-103">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0e8d6-104">ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร</span><span class="sxs-lookup"><span data-stu-id="0e8d6-104">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="0e8d6-105">สำหรับข้อมูลเพิ่มเติมโปรดเยี่ยมชมที่ลิงค์ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="0e8d6-105">For more information please visit the links below:</span></span>

- [<span data-ttu-id="0e8d6-106">หลีกเลี่ยงการควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="0e8d6-106">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="0e8d6-107">การย้ายข้อมูลและการควบคุมปริมาณ SPO</span><span class="sxs-lookup"><span data-stu-id="0e8d6-107">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="0e8d6-108">SharePoint แบบออนไลน์และความเร็วในการโยกย้าย OneDrive</span><span class="sxs-lookup"><span data-stu-id="0e8d6-108">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- <span data-ttu-id="0e8d6-109">[จัดการ SharePoint แบบออนไลน์ โดยใช้เนนเชียหลังปิดการควบคุมปริมาณ](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
[กำลังการผลิตที่วางแผน และโหลดทดสอบ SharePoint แบบออนไลน์](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)</span><span class="sxs-lookup"><span data-stu-id="0e8d6-109">[Handle SharePoint Online throttling by using exponential back off](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
[Capacity planning and load testing SharePoint Online](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)</span></span>