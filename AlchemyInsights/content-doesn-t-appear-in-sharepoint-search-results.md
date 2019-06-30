---
title: เนื้อหาที่ไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363843"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="5a0a2-102">เนื้อหาที่ไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="5a0a2-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="5a0a2-103">ทำตามขั้นตอนในการแก้ไขปัญหาเมื่อเนื้อหาที่คาดไว้ไม่ปรากฏในผลลัพธ์การค้นหา:</span><span class="sxs-lookup"><span data-stu-id="5a0a2-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="5a0a2-104">ตรวจสอบว่า**ไซต์**ที่ประกอบด้วยเนื้อหาที่คาดไว้ถูกตั้งค่าเพื่ออนุญาตให้เนื้อหาที่จะปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="5a0a2-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="5a0a2-105">ทำตามขั้นตอนในการ[แสดงเนื้อหาบนไซต์ในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="5a0a2-106">ตรวจสอบว่า**ราย**การหรือ**ไลบรารี**ที่ประกอบด้วยเนื้อหาคาดไว้ที่ถูกตั้งให้อนุญาตเนื้อหาจะปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="5a0a2-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="5a0a2-107">ทำตามขั้นตอนในการ[แสดงเนื้อหาจากรายการหรือไลบรารีในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="5a0a2-108">ตรวจสอบว่า มีการเผยแพร่หน้า เอกสาร หรือเค้าโครงเพจที่กำหนดเองเป็นแบบ**รุ่นหลัก**</span><span class="sxs-lookup"><span data-stu-id="5a0a2-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="5a0a2-109">ทำตามขั้นตอนที่ 3 ในการ[ค้นหาไม่ส่งกลับผลลัพธ์ทั้งหมดใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=874525)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="5a0a2-110">ตรวจสอบว่า ผู้ใช้มี**สิทธิ์**เพื่อดูเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="5a0a2-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="5a0a2-111">ทำตามขั้นตอนในการ[ทำความเข้าใจเกี่ยวกับระดับของสิทธิ์ใน SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="5a0a2-112">ถ้ามีการเปลี่ยนแปลง schema ค้นหา โดยการเพิ่มคุณสมบัติที่มีการจัดการใหม่ ด้วยการแก้ไขคุณสมบัติที่มีการจัดการ หรือ โดยการลบคุณสมบัติที่มีการจัดการการร้องขอการตระเวนแล้ว และจัดทำดัชนีจะไม่จำเป็น</span><span class="sxs-lookup"><span data-stu-id="5a0a2-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="5a0a2-113">**จัดทำดัชนี**เนื้อหา โดยการทำตามขั้นตอนในการ[ร้องขอการตระเวน และกำลังทำดัชนีของไซต์ ไลบรารีหรือรายการใหม่ด้วยตนเอง](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="5a0a2-114">ซึ่งอาจใช้เวลาสัก รอ 24 ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์ได้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="5a0a2-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="5a0a2-115">สำหรับข้อมูลเพิ่มเติม ดู[เปิดเนื้อหาบนไซต์ให้สามารถค้นหาได้](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="5a0a2-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
