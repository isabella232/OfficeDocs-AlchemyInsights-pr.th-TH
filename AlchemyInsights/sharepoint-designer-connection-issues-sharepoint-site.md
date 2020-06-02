---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511563"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="975f6-102">ปัญหาการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="975f6-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="975f6-103">ถ้า SharePoint Designer กําลังประสบปัญหาการเชื่อมต่อกับไซต์ SharePoint โปรดลองวิธีแก้ไขปัญหาทั่วไปต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="975f6-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="975f6-104">ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer 2013 ถูกปรับปรุง ด้วย[SharePoint ออกแบบ Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และ[2 สิงหาคม 2016 ปรับปรุงสําหรับ SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="975f6-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="975f6-105">ขั้นตอนที่ 2: ล้างแฟ้มแคชภายในเครื่อง:</span><span class="sxs-lookup"><span data-stu-id="975f6-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="975f6-106">ปิด 2013 ตัวออกแบบของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="975f6-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="975f6-107">บนคอมพิวเตอร์เฉพาะที่ เอาแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="975f6-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="975f6-108">ส่วนขยายของเว็บเซิร์ฟเวอร์\แคช</span><span class="sxs-lookup"><span data-stu-id="975f6-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="975f6-109">ตัวออกแบบของโปรแกรมประยุกต์%\Microsoft\SharePoint\พร็อกซีแอสเซมบลี</span><span class="sxs-lookup"><span data-stu-id="975f6-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="975f6-110">%โปรไฟล์ผู้ใช้%\โปรแกรมประยุกต์ข้อมูล\ภายในเครื่อง\Microsoft\เว็บไซต์การแคช</span><span class="sxs-lookup"><span data-stu-id="975f6-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="975f6-111">เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูว่าใช้งานได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="975f6-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="975f6-112">ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="975f6-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="975f6-113">ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง**อนุญาตสคริปต์แบบกําหนดเอง**ในการตั้งค่าศูนย์การจัดการ SharePoint เพื่ออนุญาตให้มีการเชื่อมต่อ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="975f6-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="975f6-114">ดู[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="975f6-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


