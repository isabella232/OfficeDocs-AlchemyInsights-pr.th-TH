---
title: เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713149"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="c0666-102">เนื้อหาไม่ปรากฏในผลลัพธ์การค้นหาของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="c0666-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="c0666-103">ทำตามขั้นตอนการแก้ไขปัญหาเหล่านี้เมื่อเนื้อหาที่คาดไว้ไม่ปรากฏในผลลัพธ์การค้นหา:</span><span class="sxs-lookup"><span data-stu-id="c0666-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="c0666-104">ตรวจสอบว่า **ไซต์** ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าเพื่ออนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="c0666-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="c0666-105">ทำตามขั้นตอนใน[แสดงเนื้อหาบนไซต์ในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="c0666-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="c0666-106">ตรวจสอบว่า **ราย** การหรือ **ไลบรารี** ที่มีเนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="c0666-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="c0666-107">ทำตามขั้นตอนใน[แสดงเนื้อหาจากรายการหรือไลบรารีในผลลัพธ์การค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)</span><span class="sxs-lookup"><span data-stu-id="c0666-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="c0666-108">ตรวจสอบว่าหน้าเอกสารหรือเค้าโครงเพจที่กำหนดเองได้รับการเผยแพร่เป็น **เวอร์ชันหลัก**</span><span class="sxs-lookup"><span data-stu-id="c0666-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="c0666-109">ทำตามขั้นตอนที่3ในการ[ค้นหาไม่ส่งกลับผลลัพธ์ทั้งหมดใน SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525)</span><span class="sxs-lookup"><span data-stu-id="c0666-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="c0666-110">ตรวจสอบว่าผู้ใช้มี **สิทธิ์** ในการดูเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="c0666-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="c0666-111">ทำตามขั้นตอนในการ[ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="c0666-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="c0666-112">ถ้า schema การค้นหาได้รับการเปลี่ยนแปลงโดยการเพิ่มคุณสมบัติที่มีการจัดการใหม่ด้วยการแก้ไขคุณสมบัติที่มีการจัดการหรือโดยการเอาคุณสมบัติที่มีการจัดการออกแล้วการร้องขอการตระเวนและการทำดัชนีใหม่จะต้องใช้</span><span class="sxs-lookup"><span data-stu-id="c0666-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="c0666-113">ทำ**ดัชนีเนื้อหาอีกครั้ง**โดยทำตามขั้นตอนในการ[ร้องขอการตระเวนด้วยตนเองและการทำดัชนีของไซต์ใหม่ไลบรารีหรือรายการ](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="c0666-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="c0666-114">การดำเนินการนี้อาจใช้เวลาสักครู่รอ24ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="c0666-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="c0666-115">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่เปิดใช้งานเนื้อหาบนไซต์เพื่อให้สามารถค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable)ได้</span><span class="sxs-lookup"><span data-stu-id="c0666-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
