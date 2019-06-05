---
title: จัดการการค้นหาพจนานุกรมใน SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 89db349189584a45c54c9c08d37ab669c3c7a39b
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716490"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="611af-102">จัดการ schema ค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="611af-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="611af-103">ค้นหา schema ควบคุมสิ่งที่ผู้ใช้สามารถค้นหา ผู้ใช้สามารถค้นหาได้ และวิธีคุณสามารถนำเสนอผลลัพธ์ในการค้นหาเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="611af-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="611af-104">เมื่อต้องการเปลี่ยนแปลง schema ค้นหา สร้างคุณสมบัติที่มีการจัดการ และแมปคุณสมบัติที่ตระเวนไปยังคุณสมบัติที่มีการจัดการ ดู[จัดการ Schema ค้นหาใน SharePoint แบบออนไลน์](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema)</span><span class="sxs-lookup"><span data-stu-id="611af-104">To change the search schema, create managed properties, and map crawled properties to managed properties, see [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema).</span></span> <span data-ttu-id="611af-105">ถ้าคุณได้รับคำเตือน 'แอพลิเคชันถูกหยุดชั่วคราว' เมื่อคุณทำการเปลี่ยนแปลง schema นี้เป็นการชั่วคราวเท่านั้นที่มีบริการบำรุงรักษาเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="611af-105">If you receive a warning 'the application is paused' when making a schema change, this is only temporary there is service maintenance occurring.</span></span> 

<span data-ttu-id="611af-106">ถ้ามีการส่งผ่านมากกว่า 24 ชั่วโมง และยังพบคำเตือน โปรดเข้าสู่ระบบสนับสนุนกรณีและปัญหา</span><span class="sxs-lookup"><span data-stu-id="611af-106">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>

<span data-ttu-id="611af-107">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการ หรือเพิ่มแท็กใหม่ เปลี่ยนแปลงมีผลเฉพาะหลังจากที่เนื้อหาถูกตระเวนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="611af-107">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="611af-108">ใน SharePoint แบบออนไลน์ ตระเวนเกิดขึ้นโดยอัตโนมัติโดยยึดตามตารางเวลาการตระเวนที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="611af-108">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>

<span data-ttu-id="611af-109">เพื่อให้แน่ใจว่า การเปลี่ยนแปลงของคุณจะมีตระเวน คุณสามารถโดยเฉพาะ[การร้องขอที่กำลังทำดัชนีใหม่ของรายการหรือไลบรารี](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="611af-109">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="611af-110">สำหรับภาพรวมที่สมบูรณ์ของ Schema ค้นหา ดู[เค้าร่างการค้นหาที่แนะนำ](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="611af-110">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 

