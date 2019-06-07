---
title: ระดับสิทธิ์ SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760711"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="054fd-102">ปัญหาการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="054fd-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="054fd-103">ถ้า SharePoint Designer ประสบปัญหาการเชื่อมต่อไปยังไซต์ SharePoint กรุณาลองแก้ไขปัญหาทั่วไปต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="054fd-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="054fd-104">ขั้นตอนที่ 1: ตรวจสอบ SharePoint Designer ถูกปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="054fd-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="054fd-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="054fd-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="054fd-106">SharePoint Designer การ Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="054fd-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="054fd-107">โปรแกรมปรับปรุงสำหรับโปรแกรมออกแบบ SharePoint 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="054fd-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="054fd-108">ขั้นตอนที่ 2: ลบแฟ้มแคชภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="054fd-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="054fd-109">ปิด SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="054fd-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="054fd-110">บนเครื่องคอมพิวเตอร์ เรียกดูไปยังโฟลเดอร์ต่อไปนี้เพื่อลบแฟ้มแคช</span><span class="sxs-lookup"><span data-stu-id="054fd-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="054fd-111">คลิกเริ่มต้น การเรียกใช้และลบแฟ้มทั้งหมดที่พบภายใต้แต่ละอยู่ด้านล่างตำแหน่งที่ตั้ง</span><span class="sxs-lookup"><span data-stu-id="054fd-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="054fd-112">เซิร์ฟเวอร์ %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="054fd-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="054fd-113">เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูถ้าทำงาน</span><span class="sxs-lookup"><span data-stu-id="054fd-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="054fd-114">ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="054fd-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="054fd-115">ขั้นตอนที่ 4: ผู้ดูแลจะต้องใช้เมื่อต้องการอนุญาตให้ใช้สคริปต์แบบกำหนดเองเพื่ออนุญาตการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="054fd-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="054fd-116">สำหรับขั้นตอนโดยละเอียด ตัวอย่าง และข้อควรพิจารณาดู[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="054fd-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


