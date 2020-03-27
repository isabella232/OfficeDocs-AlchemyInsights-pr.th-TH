---
title: ลบไซต์ใน SharePoint อย่างถาวร
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955234"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="d8ebc-102">ลบไซต์ใน SharePoint อย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="d8ebc-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="d8ebc-103">เมื่อต้องการนํา URL จากไซต์ที่ถูกลบไปมาใช้ใหม่ (เพื่อสร้างไซต์ใหม่) หรือการลบไซต์อย่างถาวร เนื่องจากไซต์นั้นไม่ได้ใช้อยู่อีกต่อไป**Permanently Delete**</span><span class="sxs-lookup"><span data-stu-id="d8ebc-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="d8ebc-104">ไปที่หน้า[ไซต์ที่ถูกลบ ของศูนย์การจัดการ SharePoint ใหม่](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)แล้วลงชื่อเข้าใช้ด้วยบัญชีที่มีสิทธิ์ระดับผู้ดูแลระบบสําหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="d8ebc-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="d8ebc-105">ในคอลัมน์ด้านซ้าย ให้เลือกไซต์</span><span class="sxs-lookup"><span data-stu-id="d8ebc-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="d8ebc-106">คลิก**ลบอย่างถาวร**</span><span class="sxs-lookup"><span data-stu-id="d8ebc-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="d8ebc-107">**หมายเหตุ**: ไม่สามารถลบไซต์ที่เชื่อมต่อกับกลุ่มจากศูนย์การจัดการ SharePoint ใหม่อย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="d8ebc-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="d8ebc-108">[ลบ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)จะต้องใช้แทน</span><span class="sxs-lookup"><span data-stu-id="d8ebc-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="d8ebc-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การลบไซต์อย่างถาวร](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="d8ebc-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
