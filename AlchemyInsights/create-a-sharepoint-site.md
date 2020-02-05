---
title: สร้างไซต์ SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770874"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="71f02-102">สร้างไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="71f02-102">Create a SharePoint site</span></span>

<span data-ttu-id="71f02-103">สร้างหรือจัดการไซต์จาก[ไซต์ที่ใช้งานอยู่](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)ในศูนย์ดูแล SharePoint</span><span class="sxs-lookup"><span data-stu-id="71f02-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="71f02-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การจัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="71f02-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="71f02-105">เคล็ด ลับ:</span><span class="sxs-lookup"><span data-stu-id="71f02-105">Tips:</span></span>

- <span data-ttu-id="71f02-106">คุณ**ไม่สามารถ**สร้างไซต์ที่มี URL เดียวกันของไซต์ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="71f02-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="71f02-107">ถ้าคุณลบไซต์และต้องการใช้ URL อีกครั้งอาจเป็นไปได้ว่าไซต์ที่ถูกลบนั้นยังคงอยู่ภายใต้[ไซต์ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)</span><span class="sxs-lookup"><span data-stu-id="71f02-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="71f02-108">ไซต์จะต้องถูกลบออกอย่างถาวรเพื่อใช้ URL อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="71f02-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="71f02-109">เมื่อต้องการเอาไซต์ออกด้วย Powershell ให้ดูที่ตัวอย่างของ cmdlet [SPSite เอาออก](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="71f02-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="71f02-110">ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="71f02-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="71f02-111">[ดูจัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="71f02-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="71f02-112">มันเป็นไปได้ว่าเว็บไซต์ปรากฏติดอยู่ที่การ**สร้าง**นานกว่าที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="71f02-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="71f02-113">ถ้ามากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="71f02-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="71f02-114">ในหลายกรณีเรากำลังหาทางแก้ไขปัญหาอยู่</span><span class="sxs-lookup"><span data-stu-id="71f02-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="71f02-115">กรุณาให้เราอย่างน้อย24ชั่วโมงเพื่อให้การแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="71f02-115">Please give us at least 24 hours to complete a solution.</span></span>
