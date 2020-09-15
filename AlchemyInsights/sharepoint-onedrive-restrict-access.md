---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700474"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="96380-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="96380-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="96380-103">มีหลายวิธีในการจำกัดการเข้าถึงบริการ SharePoint Online/OneDrive</span><span class="sxs-lookup"><span data-stu-id="96380-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="96380-104">วิธีการจำกัดการเข้าถึงต่างๆเหล่านี้จะมีการระบุไว้ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="96380-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="96380-105">**ข้อจำกัดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="96380-105">**Permission Restriction**</span></span>

<span data-ttu-id="96380-106">ใน SharePoint Online และ OneDrive for Business เราจะจำกัดการเข้าถึงรายการเช่นไซต์ไฟล์และโฟลเดอร์โดยการอนุญาตให้เข้าถึงกลุ่มเหล่านั้น/บุคคลที่ควรมีสิทธิ์เข้าถึงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="96380-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="96380-107">กำหนดสิทธิ์สำหรับรายการหรือไลบรารี SharePoint เอง</span><span class="sxs-lookup"><span data-stu-id="96380-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="96380-108">กำหนดสิทธิ์ของไซต์ SharePoint เอง</span><span class="sxs-lookup"><span data-stu-id="96380-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="96380-109">การเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย</span><span class="sxs-lookup"><span data-stu-id="96380-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="96380-110">การควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="96380-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="96380-111">ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลางคุณสามารถบล็อกหรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ไม่มีการเข้าร่วมโฆษณาแบบไฮบริดหรือเข้ากันได้ใน Intune)</span><span class="sxs-lookup"><span data-stu-id="96380-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="96380-112">**ข้อจำกัดของตำแหน่งบนเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="96380-112">**Network Location Restriction**</span></span>

<span data-ttu-id="96380-113">ในฐานะผู้ดูแลระบบ IT คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่ายที่กำหนดไว้ที่คุณเชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="96380-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="96380-114">ซึ่งเรียกว่านโยบายที่ยึดตามตำแหน่งที่ตั้ง</span><span class="sxs-lookup"><span data-stu-id="96380-114">This is also known as location-based policy.</span></span> <span data-ttu-id="96380-115">สำหรับข้อมูลเพิ่มเติมโปรดดู [ที่การควบคุมการเข้าถึงข้อมูล SharePoint Online และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="96380-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="96380-116">**ข้อจำกัดของการล็อกไซต์**</span><span class="sxs-lookup"><span data-stu-id="96380-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="96380-117">ภายใน SharePoint Online คุณจะสามารถล็อกไซต์คอลเลกชันได้ดังนั้นจึงไม่มีสิทธิ์ในการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="96380-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="96380-118">การตั้งค่านี้จะถูกตั้งค่าผ่านทาง PowerShell และการ [จัดการ SharePoint Online Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) โดยใช้คุณสมบัติ [get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState</span><span class="sxs-lookup"><span data-stu-id="96380-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="96380-119">**จำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**</span><span class="sxs-lookup"><span data-stu-id="96380-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="96380-120">ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลางคุณสามารถทำให้ผู้ใช้ของคุณสามารถสร้างและจัดการไซต์ SharePoint ของตนเองได้ซึ่งจะกำหนดชนิดของไซต์ที่พวกเขาสามารถสร้างและระบุตำแหน่งที่ตั้งของไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="96380-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="96380-121">สำหรับข้อมูลเพิ่มเติมโปรดดู [ที่จัดการการสร้างไซต์ใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="96380-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

