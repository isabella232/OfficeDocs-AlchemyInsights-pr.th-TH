---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727190"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7bc11-102">ปัญหาการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="7bc11-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7bc11-103">ถ้า SharePoint Designer กำลังประสบปัญหาการเชื่อมต่อกับไซต์ SharePoint โปรดลองใช้วิธีแก้ไขปัญหาทั่วไปต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7bc11-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="7bc11-104">ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer ๒๐๑๓ได้รับการอัปเดตด้วย[Sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และการ[อัปเดตประจำเดือนสิงหาคม 2, ๒๐๑๖สำหรับ SharePoint Designer ๒๐๑๓](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="7bc11-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="7bc11-105">ขั้นตอนที่ 2: ล้างไฟล์แคชภายในเครื่อง:</span><span class="sxs-lookup"><span data-stu-id="7bc11-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="7bc11-106">ปิด SharePoint Designer ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="7bc11-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="7bc11-107">บนคอมพิวเตอร์ที่ใช้อยู่ให้เอาไฟล์ทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้ออก</span><span class="sxs-lookup"><span data-stu-id="7bc11-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="7bc11-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="7bc11-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="7bc11-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="7bc11-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="7bc11-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="7bc11-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="7bc11-111">เปิด SharePoint Designer ๒๐๑๓แล้วใส่บัญชีผู้ใช้อีกครั้งเพื่อดูว่าทำงานหรือไม่</span><span class="sxs-lookup"><span data-stu-id="7bc11-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7bc11-112">ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องที่ทันสมัยสำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="7bc11-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="7bc11-113">ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง **อนุญาตสคริปต์แบบกำหนดเอง** ในการตั้งค่าศูนย์การจัดการ sharepoint เพื่ออนุญาตให้มีการเชื่อมต่อ sharepoint Designer</span><span class="sxs-lookup"><span data-stu-id="7bc11-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="7bc11-114">ให้ดูที่ [อนุญาตหรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7bc11-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


