---
title: เนื้อหาไม่ปรากฏในSharePointผลลัพธ์การค้นหา
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
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081629"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>เนื้อหาไม่ปรากฏในSharePointผลลัพธ์การค้นหา

Follow these troubleshooting steps when expected content doesn't appear in search results:
  
1. ตรวจสอบว่า **ไซต์ที่มี** เนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. ตรวจสอบว่า **รายการ** หรือ **ไลบรารีที่มี** เนื้อหาที่คาดไว้ถูกตั้งค่าให้อนุญาตให้เนื้อหาปรากฏในผลลัพธ์การค้นหา Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. ตรวจสอบว่าหน้า เอกสาร หรือเค้าโครงหน้าแบบเองได้รับการประกาศเป็น **เวอร์ชันหลักแล้ว** Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. ตรวจสอบว่าผู้ใช้ **มีสิทธิ์** ดูเนื้อหาหรือไม่ Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required. **Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content). การดําเนินการนี้อาจใช้เวลาสักครู่ โปรดรอ 24 ชั่วโมงก่อนที่จะตรวจสอบผลลัพธ์อีกครั้ง

For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
