---
title: เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705680"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="09db6-102">เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="09db6-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="09db6-103">ทําตามขั้นตอนการแก้ไขปัญหาเหล่านี้เมื่อเนื้อหาที่คาดไว้ไม่ปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="09db6-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="09db6-104">ตรวจสอบว่า**ไซต์**ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="09db6-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="09db6-105">ทําตามขั้นตอนใน[แสดงเนื้อหาบนไซต์ใน ผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="09db6-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="09db6-106">ตรวจสอบว่า**รายการ**หรือ**ไลบรารี**ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="09db6-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="09db6-107">ทําตามขั้นตอนใน[แสดงเนื้อหาจากรายการหรือไลบรารีในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="09db6-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="09db6-108">ตรวจสอบว่า มีการเผยแพร่เพจ เอกสาร หรือเค้าโครงเพจแบบกําหนดเองเป็น**รุ่นหลัก**</span><span class="sxs-lookup"><span data-stu-id="09db6-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="09db6-109">ทําตามขั้นตอนที่ 3 ในการค้นหา[ไม่ส่งกลับผลลัพธ์ทั้งหมดใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=874525)</span><span class="sxs-lookup"><span data-stu-id="09db6-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="09db6-110">ตรวจสอบว่า**ผู้ใช้มีสิทธิ์ดู**เนื้อหา</span><span class="sxs-lookup"><span data-stu-id="09db6-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="09db6-111">ทําตามขั้นตอนใน[ทําความเข้าใจระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="09db6-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="09db6-112">ถ้า Schema การค้นหามีการเปลี่ยนแปลงโดยการเพิ่มคุณสมบัติที่มีการจัดการใหม่</span><span class="sxs-lookup"><span data-stu-id="09db6-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="09db6-113">**ทําดัชนีเนื้อหาอีกครั้ง**โดยทําตามขั้นตอนใน[การร้องขอการตระเวนและการทําดัชนีไซต์](https://docs.microsoft.com/sharepoint/crawl-site-content)ไลบรารี หรือรายการอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="09db6-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="09db6-114">อาจใช้เวลาสักครู่รอ 24 ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="09db6-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="09db6-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[เปิดใช้งานเนื้อหาบนไซต์เพื่อให้สามารถค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable)ได้</span><span class="sxs-lookup"><span data-stu-id="09db6-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
