---
title: การสร้างไซต์ SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806958"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="d313b-102">การสร้างไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="d313b-102">Create a SharePoint site</span></span>

<span data-ttu-id="d313b-103">สร้างหรือจัดการไซต์จาก [ไซต์ที่ใช้งานอยู่](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ในศูนย์การจัดการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="d313b-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="d313b-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการไซต์ในศูนย์การจัดการ SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d313b-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="d313b-105">เคล็ด</span><span class="sxs-lookup"><span data-stu-id="d313b-105">Tips:</span></span>

- <span data-ttu-id="d313b-106">คุณ **ไม่สามารถ** สร้างไซต์ด้วย URL เดียวกันของไซต์ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="d313b-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="d313b-107">ถ้าคุณลบไซต์และต้องการใช้ URL ใหม่อาจเป็นไปได้ว่าไซต์ที่ถูกลบจะยังคงอยู่ภายใต้[ไซต์ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)</span><span class="sxs-lookup"><span data-stu-id="d313b-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="d313b-108">ไซต์จะต้องถูกลบอย่างถาวรเพื่อใช้ URL ใหม่</span><span class="sxs-lookup"><span data-stu-id="d313b-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="d313b-109">เมื่อต้องการเอาไซต์ออกด้วย Powershell ให้ดูที่ตัวอย่างของ cmdlet [SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="d313b-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="d313b-110">ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="d313b-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="d313b-111">[ดูจัดการการสร้างไซต์ใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d313b-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="d313b-112">เป็นไปได้ว่าไซต์จะปรากฏอยู่ที่การ **สร้าง** นานกว่าที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="d313b-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="d313b-113">ถ้าคุณได้รับการส่งผ่านมากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="d313b-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d313b-114">ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="d313b-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d313b-115">โปรดแจ้งให้เราทราบอย่างน้อย24ชั่วโมงเพื่อให้โซลูชันเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="d313b-115">Please give us at least 24 hours to complete a solution.</span></span>
