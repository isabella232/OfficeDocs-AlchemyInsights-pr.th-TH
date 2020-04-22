---
title: จํากัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692784"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f14fd-102">จํากัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="f14fd-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f14fd-103">มีหลายวิธีในการจํากัดการเข้าถึงบริการแบบออนไลน์/OneDrive ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="f14fd-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f14fd-104">วิธีการจํากัดการเข้าถึงต่างๆ เหล่านี้มีรายละเอียดด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="f14fd-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f14fd-105">**ข้อจํากัดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="f14fd-105">**Permission Restriction**</span></span>

<span data-ttu-id="f14fd-106">ใน SharePoint Online และ OneDrive สําหรับธุรกิจ เราจํากัดการเข้าถึงรายการต่างๆ เช่น ไซต์ ไฟล์ และโฟลเดอร์โดยการอนุญาตให้เข้าถึงกลุ่ม/บุคคลที่ควรมีสิทธิ์เข้าถึงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f14fd-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f14fd-107">กําหนดสิทธิ์สําหรับไลบรารีหรือรายการ SharePoint เอง</span><span class="sxs-lookup"><span data-stu-id="f14fd-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f14fd-108">การกําหนดสิทธิ์สําหรับไซต์ SharePoint เอง</span><span class="sxs-lookup"><span data-stu-id="f14fd-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f14fd-109">เปลี่ยนสิทธิ์บนโฟลเดอร์ย่อย</span><span class="sxs-lookup"><span data-stu-id="f14fd-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f14fd-110">ควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="f14fd-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f14fd-111">ในฐานะ SharePoint หรือผู้ดูแลระบบส่วนกลาง คุณสามารถบล็อกหรือจํากัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ผู้ที่ไม่ไฮบริดโฆษณาเข้าร่วมหรือเข้ากันได้ใน Intune)</span><span class="sxs-lookup"><span data-stu-id="f14fd-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f14fd-112">**การจํากัดตําแหน่งบนเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="f14fd-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f14fd-113">ในฐานะผู้ดูแลระบบ IT คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive ตามตําแหน่งที่ตั้งเครือข่ายที่กําหนดที่คุณเชื่อถือ</span><span class="sxs-lookup"><span data-stu-id="f14fd-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f14fd-114">ซึ่งเรียกว่านโยบายตามตําแหน่งที่ตั้ง</span><span class="sxs-lookup"><span data-stu-id="f14fd-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f14fd-115">สําหรับข้อมูลเพิ่มเติม โปรดดู[ควบคุมการเข้าถึงแบบออนไลน์ของ SharePoint และ OneDrive ข้อมูลตามตําแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f14fd-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f14fd-116">**ข้อจํากัดการล็อกไซต์**</span><span class="sxs-lookup"><span data-stu-id="f14fd-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f14fd-117">ภายใน SharePoint Online คุณสามารถล็อกไซต์คอลเลกชันได้</span><span class="sxs-lookup"><span data-stu-id="f14fd-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f14fd-118">ตั้งค่านี้ผ่านทาง PowerShell และ[เชลล์จัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้การตั้งค่า[SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState คุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="f14fd-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f14fd-119">**จํากัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**</span><span class="sxs-lookup"><span data-stu-id="f14fd-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f14fd-120">ในฐานะผู้ดูแลระบบ SharePoint หรือผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="f14fd-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f14fd-121">สําหรับข้อมูลเพิ่มเติม โปรดดู[การจัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f14fd-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

