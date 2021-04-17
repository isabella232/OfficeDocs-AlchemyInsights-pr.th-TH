---
title: ลบไซต์รากของ SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815490"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="e4eff-102">ลบไซต์รากของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="e4eff-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="e4eff-103">การลบไซต์รากของ SharePoint  **ไม่ได้รับการสนับสนุน**</span><span class="sxs-lookup"><span data-stu-id="e4eff-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="e4eff-104">If the root site has already been deleted, users will experience a 404 File Not Found error when trying to access the site.</span><span class="sxs-lookup"><span data-stu-id="e4eff-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="e4eff-105">เมื่อต้องการแก้ไข ให้คืนค่าไซต์จากศูนย์การจัดการ SharePoint ใหม่โดย  [ไปที่หน้า](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  ไซต์ที่ถูกลบ เลือกไซต์ราก แล้วคลิก คืนค่า</span><span class="sxs-lookup"><span data-stu-id="e4eff-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="e4eff-106">Instead of deleting the root site, [use replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint admin center once the root site is restored.</span><span class="sxs-lookup"><span data-stu-id="e4eff-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="e4eff-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="e4eff-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>