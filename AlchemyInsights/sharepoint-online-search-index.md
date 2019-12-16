---
title: ค้นหาใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044062"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="3dce6-102">การรวบรวมข้อมูลและการจัดทำดัชนีเนื้อหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="3dce6-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="3dce6-103">เนื้อหาต้องถูกตระเวนและเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้เพื่อค้นหาสิ่งที่กำลังค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="3dce6-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="3dce6-104">เนื้อหาจะถูกตระเวนโดยอัตโนมัติตามกำหนดการรวบรวมข้อมูลที่กำหนดไว้ล่วงหน้า (ไม่สามารถเปลี่ยนแปลงกำหนดการรวบรวมข้อมูลได้)</span><span class="sxs-lookup"><span data-stu-id="3dce6-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="3dce6-105">โปรแกรมรวบรวมข้อมูลจะรับเนื้อหาที่มีการเปลี่ยนแปลงนับตั้งแต่การตระเวนครั้งล่าสุดและปรับปรุงดัชนี</span><span class="sxs-lookup"><span data-stu-id="3dce6-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="3dce6-106">เพื่อให้แน่ใจว่าเนื้อหาถูกตระเวนและมีการปรับปรุงดัชนีให้สังเกตดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3dce6-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="3dce6-107">ตรวจสอบให้แน่ใจว่าสามารถค้นหาเนื้อหาได้โดย[ทำให้เนื้อหาไซต์ค้น](https://docs.microsoft.com/sharepoint/make-site-content-searchable)พบได้</span><span class="sxs-lookup"><span data-stu-id="3dce6-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="3dce6-108">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการหรือเมื่อคุณเปลี่ยนแปลงการแม็พของคุณสมบัติที่ถูกตระเวนและมีการจัดการไซต์จะต้องถูกตระเวนใหม่ก่อนที่การเปลี่ยนแปลงของคุณจะปรากฏในดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="3dce6-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="3dce6-109">เนื่องจากมีการเปลี่ยนแปลงของคุณในแบบแผนการค้นหาและไม่ใช่กับไซต์ที่เกิดขึ้นจริง crawler จะไม่จัดทำดัชนีไซต์อีกครั้งโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="3dce6-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="3dce6-110">สำหรับข้อมูลเพิ่มเติมให้ดู[การร้องขอการรวบรวมข้อมูลด้วยตนเองและการทำดัชนีของไซต์ใหม่ไลบรารีหรือรายการ](https://docs.microsoft.com/sharepoint/crawl-site-conten)</span><span class="sxs-lookup"><span data-stu-id="3dce6-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="3dce6-111">รออย่างน้อย24ชั่วโมงหลังจากร้องขอการรวบรวมข้อมูลด้วยตนเองและดัชนีใหม่ทั้งหมดเพื่อดูว่าคุณยังคงประสบปัญหาอยู่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="3dce6-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="3dce6-112">ถ้ามากกว่า24ชั่วโมงผ่านไปนับตั้งแต่ที่คุณเริ่มต้นการรวบรวมข้อมูลและดัชนีใหม่ทั้งหมดโปรดล็อกกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="3dce6-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="3dce6-113">ในหลายกรณีเรากำลังทำงานอยู่แล้วในการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="3dce6-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3dce6-114">กรุณาให้เราอย่างน้อย24ชั่วโมงในการดำเนินการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="3dce6-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3dce6-115">ถ้าไซต์เอกสาร (ไลบรารี) หรือรายการถูกลบและยังคงแสดงอยู่ในผลลัพธ์การค้นหาผู้ใช้ควรได้รับ**ข้อผิดพลาด๔๐๔ไม่พบแฟ้ม**เมื่อพยายามเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="3dce6-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="3dce6-116">ปัญหานี้ควรถูกบันทึกเป็นกรณีการสนับสนุนสำหรับการสืบสวนต่อไป</span><span class="sxs-lookup"><span data-stu-id="3dce6-116">This issue should be logged as a support case for further investigation.</span></span> 



