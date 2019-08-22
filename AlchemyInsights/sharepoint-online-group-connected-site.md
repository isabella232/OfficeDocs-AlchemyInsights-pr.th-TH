---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507866"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="bafeb-102">ปัญหาเมื่อสร้างหรือกลุ่มไซต์ใน SharePoint แบบออนไลน์ที่เชื่อมต่ออยู่</span><span class="sxs-lookup"><span data-stu-id="bafeb-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="bafeb-103">มีอยู่สองของปัญหาทั่วไปที่พบในขณะที่สร้าง หรือสร้างกลุ่มใหม่ให้เชื่อมต่อไซต์</span><span class="sxs-lookup"><span data-stu-id="bafeb-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="bafeb-104">ถ้าคุณได้ลบกลุ่มและไซต์เชื่อมต่ออยู่ และต้องการที่สร้างไซต์อื่นที่ มี URL เดียวกัน คุณจำเป็นต้องการเอาไซต์ก่อนหน้า</span><span class="sxs-lookup"><span data-stu-id="bafeb-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="bafeb-105">ดาวน์โหลด[SPO จัดการ Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="bafeb-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="bafeb-106">สำหรับข้อมูลเพิ่มเติมในการเริ่มต้นใช้ powershell ดู[การเริ่มต้นใช้งานกับเชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="bafeb-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="bafeb-107">เอาไซต์ออกจากไซต์ถูกลบโดยใช้ cmdlet powershell[เอา SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="bafeb-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="bafeb-108">ถ้าคุณกำลังสร้างกลุ่มเชื่อมต่อไซต์ และได้รับคำเตือนกลุ่มอื่น ด้วยนามแฝงเหมือนกันอยู่แล้ว ตรวจสอบกลุ่มจาก[Office 365 จากศูนย์ดูแล](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)ที่มีอยู่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="bafeb-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="bafeb-109">เมื่อต้องการแก้ไขปัญหา ไม่จำเป็นต้องลบกลุ่มที่มีอยู่ หรือสร้างไซต์ ด้วยนามแฝงแตกต่างกันกำหนด</span><span class="sxs-lookup"><span data-stu-id="bafeb-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="bafeb-110">มีวิธีต่าง ๆ ในการสร้าง และใช้กลุ่มสมัยใหม่กับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="bafeb-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="bafeb-111">คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Office 365</span><span class="sxs-lookup"><span data-stu-id="bafeb-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="bafeb-112">สำหรับข้อมูลเพิ่มเติม ให้ดู[กลุ่ม Office 365 ineterface ผู้ใช้ SharePoint โดยใช้การเชื่อมต่อ](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="bafeb-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="bafeb-113">เมื่อต้องการสร้างการเชื่อมโยงไซต์กลุ่ม Office 365 คุณจำเป็นต้องสร้างไซต์สำหรับทีม</span><span class="sxs-lookup"><span data-stu-id="bafeb-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="bafeb-114">สำหรับข้อมูลเพิ่มเติม โปรดดู[สร้างไซต์สำหรับทีมใน SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)</span><span class="sxs-lookup"><span data-stu-id="bafeb-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

