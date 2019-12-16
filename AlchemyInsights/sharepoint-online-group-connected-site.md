---
title: การเพิ่มกลุ่มลงในไซต์ SharePoint
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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051120"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="5787f-102">ปัญหาเมื่อสร้างหรือจัดกลุ่มไซต์ที่เชื่อมต่อใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="5787f-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="5787f-103">มีปัญหาที่พบบ่อยสองประการที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกับกลุ่มใหม่</span><span class="sxs-lookup"><span data-stu-id="5787f-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="5787f-104">หากคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นด้วย URL เดียวกันคุณจะต้องเอาไซต์ก่อนหน้าออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="5787f-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="5787f-105">ดาวน์โหลด[เชลล์จัดการการบริหาร](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="5787f-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="5787f-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน powershell โปรดดูที่[การเริ่มต้นใช้งานเชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="5787f-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="5787f-107">เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ cmdlet powershell ของการ[เอาออก SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="5787f-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="5787f-108">หากคุณกำลังสร้างไซต์ที่เชื่อมต่อกับกลุ่มและได้รับคำเตือนกลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้วให้ตรวจสอบกลุ่มที่มีอยู่จาก[Office ๓๖๕จากศูนย์การจัดการ](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)</span><span class="sxs-lookup"><span data-stu-id="5787f-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="5787f-109">เมื่อต้องการแก้ไขปัญหานี้ให้ลบกลุ่มที่มีอยู่ถ้าไม่ต้องการอีกต่อไปหรือสร้างไซต์ด้วยนามแฝงอื่นที่กำหนดไว้</span><span class="sxs-lookup"><span data-stu-id="5787f-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="5787f-110">มีหลายวิธีในการสร้างและใช้กลุ่มที่ทันสมัยกับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="5787f-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="5787f-111">คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับกลุ่ม Office ๓๖๕ได้</span><span class="sxs-lookup"><span data-stu-id="5787f-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="5787f-112">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[การเชื่อมต่อกลุ่ม Office ๓๖๕โดยใช้ ineterface ผู้ใช้ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="5787f-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="5787f-113">หากต้องการสร้างไซต์ที่เชื่อมต่อกับกลุ่ม Office ๓๖๕คุณจะต้องสร้างไซต์ทีม</span><span class="sxs-lookup"><span data-stu-id="5787f-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="5787f-114">สำหรับข้อมูลเพิ่มเติมให้ดู[สร้างไซต์ทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)</span><span class="sxs-lookup"><span data-stu-id="5787f-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

