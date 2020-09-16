---
title: จัดการ schema การค้นหาใน SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770570"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="349ad-102">จัดการ schema การค้นหาใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="349ad-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="349ad-103">Schema การค้นหาจะควบคุมสิ่งที่ผู้ใช้สามารถค้นหาวิธีที่ผู้ใช้สามารถค้นหาได้และวิธีที่คุณสามารถนำเสนอผลลัพธ์บนเว็บไซต์การค้นหาของคุณได้</span><span class="sxs-lookup"><span data-stu-id="349ad-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="349ad-104">ให้ดูที่ [จัดการ Schema การค้นหาใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) เพื่อเรียนรู้วิธีการ:</span><span class="sxs-lookup"><span data-stu-id="349ad-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="349ad-105">เปลี่ยน schema การค้นหา</span><span class="sxs-lookup"><span data-stu-id="349ad-105">Change the search schema.</span></span>
- <span data-ttu-id="349ad-106">สร้างคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="349ad-106">Create managed properties.</span></span>
- <span data-ttu-id="349ad-107">แมปแผนที่ที่ตระเวนคุณสมบัติที่ตระเวนไปยังคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="349ad-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="349ad-108">โปรดสังเกตสิ่งต่อไปนี้ในส่วนที่เกี่ยวข้องกับการจัดการ Schema การค้นหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="349ad-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="349ad-109">ถ้าคุณได้รับคำเตือนที่ระบุว่า **แอปพลิเคชันถูกหยุดชั่วคราว** เมื่อทำการเปลี่ยนแปลง schema การดำเนินการนี้จะเป็นการชั่วคราวเท่านั้นเนื่องจากมีการบำรุงรักษาบริการที่เกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="349ad-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="349ad-110">ถ้ามากกว่า24ชั่วโมงที่ผ่านมาและคุณยังคงพบคำเตือนโปรดเข้าสู่ระบบกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="349ad-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="349ad-111">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการหรือเพิ่มการเปลี่ยนแปลงจะมีผลต่อหลังจากที่เนื้อหาถูกตระเวนใหม่</span><span class="sxs-lookup"><span data-stu-id="349ad-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="349ad-112">ใน SharePoint Online การตระเวนจะเกิดขึ้นโดยอัตโนมัติโดยยึดตามกำหนดการการตระเวนที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="349ad-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="349ad-113">เมื่อต้องการตรวจสอบให้แน่ใจว่าการเปลี่ยนแปลงของคุณถูกตระเวนคุณสามารถ[ร้องขอการทำดัชนีของรายการหรือไลบรารี](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)ได้โดยเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="349ad-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="349ad-114">สำหรับภาพรวมที่สมบูรณ์ของ Schema การค้นหาให้ดูที่การ [แนะนำ schema การค้นหา](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="349ad-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


