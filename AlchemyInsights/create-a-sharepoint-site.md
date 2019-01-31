---
title: การสร้างไซต์ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 92bb7b5f0a684936db52f6be9e00c8dff3378bb5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657522"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="382b7-102">การสร้างไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="382b7-102">Create a SharePoint site</span></span>

<span data-ttu-id="382b7-p101">ดูการ[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation )สำหรับตัวเลือกการสร้างไซต์ เลือกเพื่อสร้าง[ไซต์สำหรับทีม](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US)(ซึ่งจะสร้างกลุ่ม Office 365) หรือ[ไซต์การสื่อสาร](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) การสร้าง[ไซต์แบบคลาสสิก](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)หรือไซต์ทีมใหม่ที่ไม่มีกลุ่มที่มี Office 365 คลิก**ตัวเลือกอื่น ๆ**</span><span class="sxs-lookup"><span data-stu-id="382b7-p101">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options. Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span> 
  
<span data-ttu-id="382b7-106">เคล็ดลับ:</span><span class="sxs-lookup"><span data-stu-id="382b7-106">Tips:</span></span>
- <span data-ttu-id="382b7-107">*คุณไม่สามารถสร้างไซต์ ด้วย URL ของไซต์ที่มีอยู่เดิม ถ้าคุณลบไซต์ และขอให้ใช้ URL อีกครั้ง คุณสามารถได้ในไซต์ที่ถูกลบยังคงอยู่ภายใต้\*\*ไซต์ถูกลบ*\* จัดการลบไซต์ดู[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) เมื่อต้องการเอาไซต์ ด้วย Powershell ดูตัวอย่างการ cmdlet [SPSite เอา](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)\*</span><span class="sxs-lookup"><span data-stu-id="382b7-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="382b7-108">*ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ ดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)*</span><span class="sxs-lookup"><span data-stu-id="382b7-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="382b7-109">*คุณสามารถได้ไซต์ปรากฏขึ้นติดที่**สร้าง**นานกว่าที่คาดไว้ ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์*</span><span class="sxs-lookup"><span data-stu-id="382b7-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
