---
title: จัดการเค้าร่างการค้นหาใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042982"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="9017d-102">จัดการเค้าร่างการค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="9017d-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="9017d-103">เค้าร่างการค้นหาจะควบคุมสิ่งที่ผู้ใช้สามารถค้นหาได้วิธีที่ผู้ใช้สามารถค้นหาได้และวิธีที่คุณสามารถแสดงผลบนเว็บไซต์การค้นหาของคุณ</span><span class="sxs-lookup"><span data-stu-id="9017d-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="9017d-104">ดู[จัดการแบบแผนการค้นหาใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-search-schema)เพื่อเรียนรู้วิธีการ:</span><span class="sxs-lookup"><span data-stu-id="9017d-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="9017d-105">เปลี่ยนแปลงเค้าร่างการค้นหา</span><span class="sxs-lookup"><span data-stu-id="9017d-105">Change the search schema.</span></span>
- <span data-ttu-id="9017d-106">สร้างคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="9017d-106">Create managed properties.</span></span>
- <span data-ttu-id="9017d-107">แม็ปการตระเวนแมปคุณสมบัติที่ถูกตระเวนไปยังคุณสมบัติที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="9017d-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="9017d-108">หมายเหตุต่อไปนี้ในเรื่องเกี่ยวกับการจัดการ Schema ค้นหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="9017d-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="9017d-109">ถ้าคุณได้รับคำเตือนที่ระบุว่า**แอพลิเคชันถูกหยุดการ**ทำงานเมื่อมีการเปลี่ยนแปลงเค้าร่างนี้เป็นเพียงแค่แบบถาวรเท่านั้นที่มีการบำรุงรักษาบริการเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="9017d-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="9017d-110">ถ้ามากกว่า24ชั่วโมงผ่านไปและคุณยังคงพบคำเตือนโปรดบันทึกกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="9017d-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="9017d-111">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการหรือเพิ่มแฟ้มใหม่การเปลี่ยนแปลงจะมีผลเฉพาะหลังจากที่เนื้อหาได้ถูกตระเวนใหม่</span><span class="sxs-lookup"><span data-stu-id="9017d-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="9017d-112">ใน SharePoint แบบออนไลน์การตระเวนจะเกิดขึ้นโดยอัตโนมัติตามกำหนดการรวบรวมข้อมูลที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="9017d-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="9017d-113">เพื่อให้แน่ใจว่าการเปลี่ยนแปลงของคุณถูกตระเวนคุณสามารถ[ร้องขอการทำดัชนีรายการหรือไลบรารีใหม่](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)ได้โดยเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="9017d-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="9017d-114">สำหรับภาพรวมทั้งหมดของสคีมาการค้นหาโปรดดูที่การแนะนำสคีมาการ[ค้นหา](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="9017d-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


