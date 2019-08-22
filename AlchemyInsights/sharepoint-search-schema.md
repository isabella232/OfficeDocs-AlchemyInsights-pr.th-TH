---
title: จัดการ schema ค้นหาใน SharePoint แบบออนไลน์
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502826"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="f98a2-102">จัดการ schema ค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="f98a2-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="f98a2-103">ค้นหา schema ควบคุมสิ่งที่ผู้ใช้สามารถค้นหา ผู้ใช้สามารถค้นหาได้ และวิธีคุณสามารถนำเสนอผลลัพธ์ในการค้นหาเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f98a2-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="f98a2-104">ดูการ[จัดการ Schema ค้นหาใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-search-schema)เพื่อเรียนรู้วิธีการ:</span><span class="sxs-lookup"><span data-stu-id="f98a2-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="f98a2-105">เปลี่ยนแบบแผนการค้นหา</span><span class="sxs-lookup"><span data-stu-id="f98a2-105">Change the search schema.</span></span>
- <span data-ttu-id="f98a2-106">สร้างคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="f98a2-106">Create managed properties.</span></span>
- <span data-ttu-id="f98a2-107">แผนผังตระเวนแมปคุณสมบัติที่ตระเวนไปยังคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="f98a2-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="f98a2-108">หมายเหตุอินวอยซ์กับ Schema ของคุณค้นหาการจัดการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f98a2-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="f98a2-109">ถ้าคุณได้รับคำเตือนที่ระบุ**โปรแกรมประยุกต์ถูกหยุดชั่วคราว**เมื่อคุณทำการเปลี่ยนแปลง schema นี่คือเพียงชั่วคราวเนื่องจากมีการบำรุงรักษาบริการเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="f98a2-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="f98a2-110">ถ้ามีการส่งผ่านมากกว่า 24 ชั่วโมง และยังพบคำเตือน โปรดเข้าสู่ระบบสนับสนุนกรณีและปัญหา</span><span class="sxs-lookup"><span data-stu-id="f98a2-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="f98a2-111">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการ หรือเพิ่มแท็กใหม่ เปลี่ยนแปลงมีผลเฉพาะหลังจากที่เนื้อหาถูกตระเวนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="f98a2-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="f98a2-112">ใน SharePoint แบบออนไลน์ ตระเวนเกิดขึ้นโดยอัตโนมัติโดยยึดตามตารางเวลาการตระเวนที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="f98a2-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="f98a2-113">เพื่อให้แน่ใจว่า การเปลี่ยนแปลงของคุณจะมีตระเวน คุณสามารถโดยเฉพาะ[การร้องขอที่กำลังทำดัชนีใหม่ของรายการหรือไลบรารี](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="f98a2-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="f98a2-114">สำหรับภาพรวมที่สมบูรณ์ของ Schema ค้นหา ดู[เค้าร่างการค้นหาที่แนะนำ](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="f98a2-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


