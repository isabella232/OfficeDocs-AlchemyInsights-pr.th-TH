---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750683"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b8476-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8476-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b8476-103">มีหลายวิธีในการจำกัดการเข้าถึงบริการ SharePoint แบบออนไลน์/OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8476-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="b8476-104">วิธีการจำกัดการเข้าถึงต่างๆเหล่านี้มีการระบุไว้ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="b8476-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="b8476-105">**ข้อจำกัดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="b8476-105">**Permission Restriction**</span></span>

<span data-ttu-id="b8476-106">ใน SharePoint แบบออนไลน์และ OneDrive สำหรับธุรกิจเราจำกัดการเข้าถึงรายการต่างๆเช่นไซต์แฟ้มและโฟลเดอร์โดยการให้สิทธิ์เข้าถึงกลุ่มเหล่านั้น/บุคคลที่ควรมีการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="b8476-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="b8476-107">กำหนดสิทธิ์สำหรับรายการหรือไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="b8476-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="b8476-108">การกำหนดสิทธิ์ของไซต์ SharePoint เอง</span><span class="sxs-lookup"><span data-stu-id="b8476-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="b8476-109">การเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์ย่อย</span><span class="sxs-lookup"><span data-stu-id="b8476-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="b8476-110">ควบคุมการเข้าถึงจากอุปกรณ์ที่ไม่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="b8476-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="b8476-111">ในฐานะที่เป็น SharePoint หรือผู้ดูแลส่วนกลางใน Office ๓๖๕คุณสามารถบล็อกหรือจำกัดการเข้าถึงเนื้อหา SharePoint และ OneDrive จากอุปกรณ์ที่ไม่มีการจัดการ (ผู้ที่ไม่ได้เป็นสมาชิกไฮบริดสลีเข้าร่วมหรือสอดคล้องกันใน Intune)</span><span class="sxs-lookup"><span data-stu-id="b8476-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="b8476-112">**ข้อจำกัดตำแหน่งเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="b8476-112">**Network Location Restriction**</span></span>

<span data-ttu-id="b8476-113">ในฐานะที่เป็นผู้ดูแลระบบไอทีคุณสามารถควบคุมการเข้าถึงทรัพยากร SharePoint และ OneDrive ตามตำแหน่งบนเครือข่ายที่กำหนดไว้ที่คุณเชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="b8476-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="b8476-114">ซึ่งเรียกอีกอย่างว่านโยบายตามตำแหน่งที่ตั้ง</span><span class="sxs-lookup"><span data-stu-id="b8476-114">This is also known as location-based policy.</span></span> <span data-ttu-id="b8476-115">สำหรับข้อมูลเพิ่มเติมโปรดดู[การควบคุมการเข้าถึงข้อมูล SharePoint แบบออนไลน์และ OneDrive ตามตำแหน่งบนเครือข่าย](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="b8476-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="b8476-116">**ข้อจำกัดในการล็อกเว็บไซต์**</span><span class="sxs-lookup"><span data-stu-id="b8476-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="b8476-117">ภายใน SharePoint แบบออนไลน์คุณมีความสามารถในการล็อกชุดเก็บรวบรวมไซต์ดังนั้นไม่มีใครมีการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="b8476-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="b8476-118">นี้ถูกตั้งค่าผ่านทาง PowerShell และ[เชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)โดยใช้คุณสมบัติการ[ตั้งค่าเว็บไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)-lockstate</span><span class="sxs-lookup"><span data-stu-id="b8476-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="b8476-119">**การจำกัดผู้ใช้จากการสร้างไซต์หรือไซต์ย่อย**</span><span class="sxs-lookup"><span data-stu-id="b8476-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="b8476-120">ในฐานะที่เป็นผู้ดูแลระบบ SharePoint หรือ Office ๓๖๕ผู้ดูแลส่วนกลางคุณสามารถให้ผู้ใช้ของคุณสร้างและดูแลไซต์ SharePoint ของตนเองได้กำหนดชนิดของไซต์ที่พวกเขาสามารถสร้างและระบุตำแหน่งที่ตั้งของไซต์</span><span class="sxs-lookup"><span data-stu-id="b8476-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="b8476-121">สำหรับข้อมูลเพิ่มเติมโปรดดู[จัดการการสร้างไซต์ใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="b8476-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

