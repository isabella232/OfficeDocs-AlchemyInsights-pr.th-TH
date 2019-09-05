---
title: การสร้างไซต์ SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738216"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="27368-102">การสร้างไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="27368-102">Create a SharePoint site</span></span>

<span data-ttu-id="27368-103">คุณสามารถดูข้อมูลเกี่ยวกับการสร้างไซต์ SharePoint ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="27368-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="27368-104">[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation): เรียนรู้เกี่ยวกับตัวเลือกการสร้างไซต์รวมถึงวิธีการสร้างไซต์คลาสสิกหรือไซต์ทีมที่ไม่มีกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="27368-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="27368-105">[สร้างไซต์ทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): เรียนรู้วิธีการสร้างไซต์ทีม</span><span class="sxs-lookup"><span data-stu-id="27368-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="27368-106">[สร้างไซต์การสื่อสารใน SharePoint แบบออนไลน์](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): เรียนรู้วิธีการสร้างไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="27368-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="27368-107">[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): เรียนรู้วิธีการสร้างไซต์คลาสสิกหรือไซต์ทีมที่ไม่มีกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="27368-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="27368-108">[! เคล็ดลับ</span><span class="sxs-lookup"><span data-stu-id="27368-108">[!Tips]</span></span>
> - <span data-ttu-id="27368-109">คุณไม่สามารถสร้างไซต์ที่มี URL เดียวกันของไซต์ที่มีอยู่ได้</span><span class="sxs-lookup"><span data-stu-id="27368-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="27368-110">หากคุณลบไซต์และต้องการใช้ URL อีกครั้งอาจเป็นไปได้ว่าไซต์ที่ถูกลบยังคงอยู่ภายใต้**ไซต์ที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="27368-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="27368-111">หากต้องการจัดการไซต์ที่ถูกลบให้เห็นให้[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="27368-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="27368-112">หากต้องการเอาเว็บไซต์ที่มี Powershell ออกให้ดูตัวอย่างการ[เอาออก spsite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet</span><span class="sxs-lookup"><span data-stu-id="27368-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="27368-113">ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="27368-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="27368-114">ดู[จัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="27368-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="27368-115">เป็นไปได้ที่เว็บไซต์จะปรากฏติดอยู่ที่**การสร้าง**นานกว่าที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="27368-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="27368-116">หากมีการผ่านมากกว่า24ชั่วโมงตั้งแต่แรกคุณเห็นปัญหานี้โปรดบันทึกตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="27368-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="27368-117">ในหลายกรณีเรากำลังทำงานอยู่แล้วในการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="27368-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="27368-118">กรุณาให้เราอย่างน้อย24ชั่วโมงในการดำเนินการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="27368-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="27368-119">ถ้าคุณต้องการสร้างไซต์ทีมใหม่ที่ไม่มีกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="27368-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


