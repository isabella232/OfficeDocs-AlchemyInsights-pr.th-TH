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
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515826"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="1fde7-102">การสร้างไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="1fde7-102">Create a SharePoint site</span></span>

<span data-ttu-id="1fde7-103">คุณสามารถดูที่ด้านล่างสำหรับข้อมูลเกี่ยวกับการสร้างไซต์ SharePoint:</span><span class="sxs-lookup"><span data-stu-id="1fde7-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="1fde7-104">[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation): การเรียนรู้เกี่ยวกับตัวเลือกการสร้างไซต์ รวมทั้งวิธีการสร้างไซต์แบบคลาสสิคหรือไซต์ทีมงานที่ไม่มีกลุ่มที่มี Office 365</span><span class="sxs-lookup"><span data-stu-id="1fde7-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="1fde7-105">[การสร้างไซต์ทีม SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): การเรียนรู้วิธีการสร้างไซต์สำหรับทีม</span><span class="sxs-lookup"><span data-stu-id="1fde7-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="1fde7-106">[สร้างไซต์สื่อสารใน SharePoint แบบออนไลน์](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): เรียนรู้วิธีการสร้างไซต์สื่อสาร</span><span class="sxs-lookup"><span data-stu-id="1fde7-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="1fde7-107">[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): การเรียนรู้วิธีการสร้างไซต์แบบคลาสสิคหรือไซต์สำหรับทีมที่ไม่มีกลุ่มที่มี Office 365</span><span class="sxs-lookup"><span data-stu-id="1fde7-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! คำแนะนำ]
> - <span data-ttu-id="1fde7-109">คุณไม่สามารถสร้างไซต์ ด้วย URL ของไซต์ที่มีอยู่เดิม</span><span class="sxs-lookup"><span data-stu-id="1fde7-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="1fde7-110">ถ้าคุณลบไซต์ และขอให้ใช้ URL อีกครั้ง คุณสามารถได้ในไซต์ที่ถูกลบยังคงอยู่ภายใต้**ไซต์ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="1fde7-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="1fde7-111">จัดการลบไซต์ดู[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="1fde7-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="1fde7-112">เมื่อต้องการเอาไซต์ ด้วย Powershell ดูตัวอย่างการ cmdlet [SPSite เอา](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="1fde7-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="1fde7-113">ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="1fde7-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="1fde7-114">ดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="1fde7-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="1fde7-115">คุณสามารถได้ไซต์ปรากฏขึ้นติดที่**สร้าง**นานกว่าที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="1fde7-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="1fde7-116">ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน</span><span class="sxs-lookup"><span data-stu-id="1fde7-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1fde7-117">ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน</span><span class="sxs-lookup"><span data-stu-id="1fde7-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1fde7-118">โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="1fde7-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="1fde7-119">ถ้าคุณต้องการสร้างไซต์ทีมใหม่ที่ไม่มีกลุ่มที่มี Office 365</span><span class="sxs-lookup"><span data-stu-id="1fde7-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


