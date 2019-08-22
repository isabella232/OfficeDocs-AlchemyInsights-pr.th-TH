---
title: ค้นหาใน SharePoint แบบออนไลน์
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507650"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="dcad2-102">การตระเวนเนื้อหาและการทำดัชนีใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="dcad2-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="dcad2-103">เนื้อหาต้องตระเวน และเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้ในการค้นหาสิ่งที่กำลังค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="dcad2-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="dcad2-104">เนื้อหาถูกตระเวนโดยอัตโนมัติตามตารางเวลาการตระเวนที่กำหนดไว้ล่วงหน้า (ไม่สามารถเปลี่ยนแปลงตารางเวลาการตระเวน)</span><span class="sxs-lookup"><span data-stu-id="dcad2-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="dcad2-105">ตัวตระเวนรับค่าเนื้อหาที่มีการเปลี่ยนแปลงนับตั้งแต่การตระเวนครั้งล่าสุด และการปรับปรุงดัชนี</span><span class="sxs-lookup"><span data-stu-id="dcad2-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="dcad2-106">เพื่อให้แน่ใจว่า ตระเวนเนื้อหา และดัชนีมีการปรับปรุง หมายเหตุต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="dcad2-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="dcad2-107">ตรวจสอบให้แน่ใจว่า เนื้อหาสามารถค้นพบได้โดยการ[ทำให้สามารถค้นหาเนื้อหาไซต์](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="dcad2-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="dcad2-108">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการ หรือ เมื่อคุณได้เปลี่ยนการแม็ปตระเวน และจัดการคุณสมบัติ ไซต์ต้องถูกตระเวนอีกครั้งก่อนที่การเปลี่ยนแปลงจะมีผลต่อดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="dcad2-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="dcad2-109">เนื่องจากมีทำการเปลี่ยนแปลงของคุณใน schema ค้นหา และไม่ให้ไซต์จริง ตัวตระเวนจะไม่อัตโนมัติใหม่ดัชนีให้กับไซต์</span><span class="sxs-lookup"><span data-stu-id="dcad2-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="dcad2-110">สำหรับข้อมูลเพิ่มเติม ดู[ขอตระเวน และการทำดัชนีของไซต์ ไลบรารีหรือรายการใหม่ด้วยตนเอง](https://docs.microsoft.com/sharepoint/crawl-site-conten)</span><span class="sxs-lookup"><span data-stu-id="dcad2-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="dcad2-111">รออย่างน้อย 24 ชั่วโมงหลังจากการร้องขอการตระเวนและแบบเต็มดัชนีใหม่เมื่อต้องการดูถ้าคุณยังคงประสบกับปัญหาด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="dcad2-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="dcad2-112">ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่เริ่มต้นการตระเวนและเต็มจัดดัชนี โปรดเข้าสู่ระบบสนับสนุนกรณีและปัญหา</span><span class="sxs-lookup"><span data-stu-id="dcad2-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="dcad2-113">ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน</span><span class="sxs-lookup"><span data-stu-id="dcad2-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="dcad2-114">โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="dcad2-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dcad2-115">ถ้าไซต์ เอกสาร (ไลบรารี), หรือรายการถูกลบ และยังคง แสดงให้เห็นในผลลัพธ์การค้นหา ผู้ใช้ควรได้รับข้อ**ผิดพลาด 404 ไม่พบแฟ้ม**เมื่อพยายามเข้าถึงแฟ้มนั้น</span><span class="sxs-lookup"><span data-stu-id="dcad2-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="dcad2-116">ปัญหานี้ควรเข้าสู่ระบบเป็นกรณีและปัญหาสนับสนุนสำหรับการสืบสวนเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="dcad2-116">This issue should be logged as a support case for further investigation.</span></span> 



