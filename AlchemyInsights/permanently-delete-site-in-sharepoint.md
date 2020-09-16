---
title: ลบไซต์ใน SharePoint อย่างถาวร
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771740"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="f22b3-102">ลบไซต์ใน SharePoint อย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="f22b3-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="f22b3-103">เมื่อต้องการนำ URL มาใช้ใหม่จากไซต์ที่ถูกลบ (เมื่อต้องการสร้างไซต์ใหม่) หรือเมื่อต้องการลบไซต์อย่างถาวรเนื่องจากไม่มีการใช้งานอีกต่อไปคุณสามารถใช้การ **ลบอย่างถาวร** จากศูนย์การจัดการ SharePoint ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f22b3-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="f22b3-104">ไปที่ [หน้าไซต์ที่ถูกลบของศูนย์การจัดการ SharePoint ใหม่](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) แล้วลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีสิทธิ์ผู้ดูแลระบบสำหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="f22b3-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="f22b3-105">ในคอลัมน์ด้านซ้ายให้เลือกไซต์</span><span class="sxs-lookup"><span data-stu-id="f22b3-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="f22b3-106">คลิก**ลบอย่างถาวร**</span><span class="sxs-lookup"><span data-stu-id="f22b3-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="f22b3-107">**หมายเหตุ**: ไม่สามารถลบไซต์ที่เชื่อมต่อกับกลุ่มได้อย่างถาวรจากศูนย์การจัดการ SharePoint ใหม่</span><span class="sxs-lookup"><span data-stu-id="f22b3-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="f22b3-108">[เอาออก-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) จะต้องถูกใช้แทน</span><span class="sxs-lookup"><span data-stu-id="f22b3-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="f22b3-109">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ลบไซต์อย่างถาวร](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="f22b3-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
