---
title: เนื้อหาที่ไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 3871e2eed2e321e0df72fe3578a14ddd45ed8565
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660546"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="096b7-102">เนื้อหาที่ไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="096b7-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="096b7-103">ทำตามขั้นตอนในการแก้ไขปัญหาเมื่อเนื้อหาที่คาดไว้ไม่ปรากฏในผลลัพธ์การค้นหา:</span><span class="sxs-lookup"><span data-stu-id="096b7-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="096b7-p101">ตรวจสอบว่า**ไซต์**ที่ประกอบด้วยเนื้อหาที่คาดไว้ถูกตั้งค่าเพื่ออนุญาตให้เนื้อหาที่จะปรากฏในผลลัพธ์การค้นหา ทำตามขั้นตอนในการ[แสดงเนื้อหาบนไซต์ในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="096b7-p101">Check that the **site** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>
    
2. <span data-ttu-id="096b7-p102">ตรวจสอบว่า**ราย**การหรือ**ไลบรารี**ที่ประกอบด้วยเนื้อหาคาดไว้ที่ถูกตั้งให้อนุญาตเนื้อหาจะปรากฏในผลลัพธ์การค้นหา ทำตามขั้นตอนในการ[แสดงเนื้อหาจากรายการหรือไลบรารีในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="096b7-p102">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span> 
    
3. <span data-ttu-id="096b7-p103">ตรวจสอบว่า มีการเผยแพร่หน้า เอกสาร หรือเค้าโครงเพจที่กำหนดเองเป็นแบบ**รุ่นหลัก** ทำตามขั้นตอนที่ 3 ในการ[ค้นหาไม่ส่งกลับผลลัพธ์ทั้งหมดใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=874525)</span><span class="sxs-lookup"><span data-stu-id="096b7-p103">Verify that the page, document, or custom page layout is published as a **Major version.** Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>
    
4. <span data-ttu-id="096b7-p104">ตรวจสอบว่า ผู้ใช้มี**สิทธิ์**เพื่อดูเนื้อหา ทำตามขั้นตอนในการ[ทำความเข้าใจเกี่ยวกับระดับของสิทธิ์ใน SharePoint](https://go.microsoft.com/fwlink/?linkid=867071)</span><span class="sxs-lookup"><span data-stu-id="096b7-p104">Verify that the user has **permissions** to view the content. Follow the steps in [Understanding permission levels in SharePoint](https://go.microsoft.com/fwlink/?linkid=867071).</span></span>
    
5. <span data-ttu-id="096b7-p105">**จัดทำดัชนี**เนื้อหา โดยการทำตามขั้นตอนในการ[ร้องขอการตระเวน และกำลังทำดัชนีของไซต์ ไลบรารีหรือรายการใหม่ด้วยตนเอง](https://docs.microsoft.com/sharepoint/crawl-site-content) ซึ่งอาจใช้เวลาสัก รอ 24 ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์ได้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="096b7-p105">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content). This might take a while, wait 24 hours before checking the results again.</span></span>
    
<span data-ttu-id="096b7-114">สำหรับข้อมูลเพิ่มเติม ดู[เปิดเนื้อหาบนไซต์ให้สามารถค้นหาได้](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="096b7-114">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

