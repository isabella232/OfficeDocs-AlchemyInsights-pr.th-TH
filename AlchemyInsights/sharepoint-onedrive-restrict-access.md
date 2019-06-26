---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223731"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="17f4e-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="17f4e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="17f4e-103">มีหลายวิธีในการจำกัดการเข้าถึงบริการ ออนไลน์/OneDrive ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="17f4e-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="17f4e-104">วิธีเข้าถึงข้อจำกัดต่าง ๆ จะถูกทำเค้าร่างด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="17f4e-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="17f4e-105">**การจำกัดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="17f4e-105">**Permission Restriction**</span></span>

<span data-ttu-id="17f4e-106">ใน SharePoint แบบออนไลน์และ OneDrive สำหรับธุรกิจ เราจำกัดการเข้าถึงรายการอย่างเช่นไซต์ แฟ้ม และโฟลเดอร์ โดยเฉพาะ สิทธิการเข้าถึงกลุ่ม/ผู้ใช้เหล่านั้นควรมีการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="17f4e-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="17f4e-107">กำหนดสิทธิ์สำหรับรายการ SharePoint หรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="17f4e-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="17f4e-108">กำหนดสิทธิ์ของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="17f4e-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="17f4e-109">เปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย</span><span class="sxs-lookup"><span data-stu-id="17f4e-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="17f4e-110">ควบคุมการเข้าถึงจากอุปกรณ์ไม่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="17f4e-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="17f4e-111">เป็นผู้ดูแลส่วนกลางใน Office 365 หรือ SharePoint คุณสามารถบล็อก หรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ไม่มีการจัดการ (เหล่าไฮบริโฆษณาที่นำมารวมกัน หรือเข้ากันได้ใน Intune) ได้</span><span class="sxs-lookup"><span data-stu-id="17f4e-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="17f4e-112">**ข้อจำกัดของตำแหน่งที่ตั้งเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="17f4e-112">**Network Location Restriction**</span></span>

<span data-ttu-id="17f4e-113">เป็นผู้ดูแลระบบ IT ผิด คุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่ายที่กำหนดที่คุณเชื่อถือ</span><span class="sxs-lookup"><span data-stu-id="17f4e-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="17f4e-114">นี่คือหรือที่เรียกอีกอย่างหนึ่งว่านโยบายที่อ้างอิงตำแหน่งที่ตั้ง</span><span class="sxs-lookup"><span data-stu-id="17f4e-114">This is also known as location-based policy.</span></span> <span data-ttu-id="17f4e-115">สำหรับข้อมูลเพิ่มเติม โปรดดูที่[ควบคุมการเข้าถึงแบบออนไลน์ของ SharePoint และข้อมูล OneDrive โดยยึดตามตำแหน่งที่ตั้งเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="17f4e-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="17f4e-116">**ข้อจำกัดการล็อกไซต์**</span><span class="sxs-lookup"><span data-stu-id="17f4e-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="17f4e-117">ภายใน SharePoint แบบออนไลน์ คุณมีความสามารถในการล็อกไซต์คอลเลกชัน เพื่อให้ไม่มีผู้ใดมีสิทธิ์เข้าถึง</span><span class="sxs-lookup"><span data-stu-id="17f4e-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="17f4e-118">การกระทำนี้จะตั้งผ่านทาง PowerShell และ[เชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้คุณสมบัติ[ชุด-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState</span><span class="sxs-lookup"><span data-stu-id="17f4e-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="17f4e-119">**จำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**</span><span class="sxs-lookup"><span data-stu-id="17f4e-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="17f4e-120">เป็นผู้ดูแลระบบ SharePoint หรือผู้ดูแลส่วนกลางของ Office 365 คุณสามารถให้ผู้ใช้ของคุณสร้าง และการดูแลไซต์ SharePoint ของตนเอง กำหนดชนิดของไซต์ที่พวกเขาสามารถสร้าง และระบุที่ตั้งของไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="17f4e-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="17f4e-121">สำหรับข้อมูลเพิ่มเติม โปรดดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="17f4e-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

