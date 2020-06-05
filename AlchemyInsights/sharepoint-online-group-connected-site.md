---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582830"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="191f3-102">ปัญหาเมื่อสร้างไซต์ที่เชื่อมต่อกลุ่มใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="191f3-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="191f3-103">ปัญหาทั่วไปบางอย่างที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกลุ่มใหม่</span><span class="sxs-lookup"><span data-stu-id="191f3-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="191f3-104">ถ้าคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นที่มี URL เดียวกัน คุณจะต้องลบไซต์ก่อนหน้าอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="191f3-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="191f3-105">ดาวน์โหลด[เชลล์จัดการ SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="191f3-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="191f3-106">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้ Powershell ให้ดูที่[การเริ่มต้นใช้งานเชลล์การจัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)</span><span class="sxs-lookup"><span data-stu-id="191f3-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="191f3-107">เอาไซต์จากไซต์ที่ถูกลบโดยใช้ cmdlet ของ Powershell[ลบ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="191f3-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="191f3-108">จําเป็นต้องมี Powershell เพื่อลบไซต์กลุ่มอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="191f3-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="191f3-109">ถ้าคุณกําลังสร้างไซต์ที่เชื่อมต่อกลุ่มและได้รับคําเตือน:**มีอีกกลุ่มหนึ่งที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups)</span><span class="sxs-lookup"><span data-stu-id="191f3-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="191f3-110">เมื่อต้องการแก้ปัญหา ให้ลบกลุ่มที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="191f3-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="191f3-111">มีวิธีต่างๆ ในการสร้างและใช้กลุ่มสมัยใหม่กับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="191f3-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="191f3-112">คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="191f3-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="191f3-113">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเชื่อมต่อกลุ่ม Microsoft 365 โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="191f3-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="191f3-114">เมื่อต้องการสร้างไซต์ที่เชื่อมต่อกลุ่ม Microsoft 365 คุณจะต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="191f3-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
