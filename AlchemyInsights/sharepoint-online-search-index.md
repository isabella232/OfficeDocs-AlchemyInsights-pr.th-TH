---
title: จัดการการค้นหาพจนานุกรมใน SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758784"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="ea632-102">ค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ea632-102">Search in SharePoint Online</span></span>

<span data-ttu-id="ea632-103">เนื้อหาต้องตระเวน และเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้ในการค้นหาสิ่งที่กำลังค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ea632-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="ea632-104">เนื้อหาถูกตระเวนโดยอัตโนมัติตามตารางเวลาการตระเวนที่กำหนดไว้ล่วงหน้า (ไม่สามารถเปลี่ยนแปลงตารางเวลาการตระเวน)</span><span class="sxs-lookup"><span data-stu-id="ea632-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="ea632-105">ตัวตระเวนรับค่าเนื้อหาที่มีการเปลี่ยนแปลงนับตั้งแต่การตระเวนครั้งล่าสุด และการปรับปรุงดัชนี</span><span class="sxs-lookup"><span data-stu-id="ea632-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="ea632-106">เพื่อให้แน่ใจว่า ตระเวนเนื้อหา และมีการปรับปรุงดัชนี ทำตามขั้นตอนด้านล่างนี้</span><span class="sxs-lookup"><span data-stu-id="ea632-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="ea632-107">ตรวจสอบให้แน่ใจว่า เนื้อหาสามารถค้นพบได้ โดยการทำให้สามารถค้นหาเนื้อหาไซต์</span><span class="sxs-lookup"><span data-stu-id="ea632-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="ea632-108">สำหรับข้อมูลเพิ่มเติม ดู[เปิดเนื้อหาบนไซต์ให้สามารถค้นหาได้](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="ea632-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="ea632-109">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการ หรือ เมื่อคุณได้เปลี่ยนการแม็ปตระเวน และจัดการคุณสมบัติ ไซต์ต้องถูกตระเวนอีกครั้งก่อนที่การเปลี่ยนแปลงจะมีผลต่อดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="ea632-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="ea632-110">เนื่องจากมีทำการเปลี่ยนแปลงของคุณใน schema ค้นหา และไม่ให้ไซต์จริง ตัวตระเวนจะไม่อัตโนมัติใหม่ดัชนีให้กับไซต์</span><span class="sxs-lookup"><span data-stu-id="ea632-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="ea632-111">สำหรับข้อมูลเพิ่มเติม ดู[ขอตระเวน และการทำดัชนีของไซต์ ไลบรารีหรือรายการใหม่ด้วยตนเอง](https://docs.microsoft.com/sharepoint/crawl-site-conten)</span><span class="sxs-lookup"><span data-stu-id="ea632-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="ea632-112">รออย่างน้อย 24 ชั่วโมงหลังจากการร้องขอการตระเวนและแบบเต็มดัชนีใหม่เมื่อต้องการดูถ้าคุณยังคงประสบกับปัญหาด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="ea632-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="ea632-113">ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่เริ่มต้นการตระเวนและเต็มจัดดัชนี โปรดเข้าสู่ระบบสนับสนุนกรณีและปัญหา</span><span class="sxs-lookup"><span data-stu-id="ea632-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="ea632-114">ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน</span><span class="sxs-lookup"><span data-stu-id="ea632-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ea632-115">โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="ea632-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="ea632-116">**สิ่งสำคัญ**: หากไซต์ เอกสาร (ไลบรารี), หรือรายการถูกลบไปแล้ว และยังคงแสดงในผลลัพธ์การค้นหา ผู้ใช้ควรได้รับข้อผิดพลาด 404 ไม่พบแฟ้มเมื่อพยายามเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="ea632-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="ea632-117">ปัญหานี้ควรเข้าสู่ระบบเป็นกรณีและปัญหาสนับสนุนสำหรับการสืบสวนเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="ea632-117">This issue should be logged as a support case for further investigation.</span></span> 



