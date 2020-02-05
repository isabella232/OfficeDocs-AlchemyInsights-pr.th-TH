---
title: การเพิ่มกลุ่มให้กับไซต์ SharePoint
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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770370"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="6c803-102">ปัญหาเมื่อสร้างไซต์ที่เชื่อมต่อกับกลุ่มใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="6c803-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="6c803-103">ปัญหาทั่วไปบางอย่างที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกับกลุ่มอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="6c803-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="6c803-104">หากคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นด้วย URL เดียวกันคุณจะต้องลบไซต์ก่อนหน้านี้อย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="6c803-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="6c803-105">ดาวน์โหลด[เชลล์การจัดการ SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="6c803-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="6c803-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน Powershell ให้ดู[ที่การเริ่มต้นใช้งานเชลล์จัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)</span><span class="sxs-lookup"><span data-stu-id="6c803-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="6c803-107">เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ cmdlet Powershell[ลบ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="6c803-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="6c803-108">จำเป็นต้องมี Powershell เพื่อลบไซต์กลุ่มอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="6c803-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="6c803-109">ถ้าคุณกำลังสร้างไซต์ที่เชื่อมต่อกับกลุ่มและได้รับคำเตือน:**กลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[Office ๓๖๕จากศูนย์ดูแล](https://admin.microsoft.com/AdminPortal/Home#/groups)</span><span class="sxs-lookup"><span data-stu-id="6c803-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="6c803-110">เมื่อต้องการแก้ไขปัญหานี้ให้ลบกลุ่มที่มีอยู่ถ้าไม่จำเป็นหรือสร้างไซต์ด้วยนามแฝงที่แตกต่างกันที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="6c803-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="6c803-111">มีหลายวิธีในการสร้างและใช้กลุ่มที่ทันสมัยกับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6c803-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="6c803-112">คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="6c803-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="6c803-113">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การเชื่อมต่อกลุ่ม Office ๓๖๕โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="6c803-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="6c803-114">เมื่อต้องการสร้างไซต์ที่เชื่อมต่อกับกลุ่ม Office ๓๖๕คุณจะต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="6c803-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
