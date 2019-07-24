---
title: ปัญหาการเชื่อมต่อของ SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840570"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7663c-102">ปัญหาการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="7663c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7663c-103">ถ้า SharePoint Designer ประสบปัญหาการเชื่อมต่อไปยังไซต์ SharePoint กรุณาลองแก้ไขปัญหาทั่วไปต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7663c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="7663c-104">ขั้นตอนที่ 1: ตรวจสอบว่า มีการปรับปรุง SharePoint Designer 2013 มีค่า[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 สิงหาคม 2016 ปรับปรุง SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="7663c-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="7663c-105">ขั้นตอนที่ 2: ลบแฟ้มแคชภายในเครื่อง:</span><span class="sxs-lookup"><span data-stu-id="7663c-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="7663c-106">ปิด SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="7663c-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="7663c-107">บนเครื่องคอมพิวเตอร์ ลบแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7663c-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="7663c-108">Extensions\Cache เซิร์ฟเวอร์ %APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="7663c-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="7663c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="7663c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="7663c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="7663c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="7663c-111">เปิด SharePoint Designer 2013 และป้อนบัญชีอีกครั้งเพื่อดูถ้าทำงาน</span><span class="sxs-lookup"><span data-stu-id="7663c-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7663c-112">ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7663c-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="7663c-113">ขั้นตอนที่ 4: ผู้ดูแลจะต้อง**อนุญาตให้สคริปต์แบบกำหนดเอง**ในการตั้งค่าศูนย์กลางการดูแล SharePoint เพื่ออนุญาตการเชื่อมต่อของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="7663c-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="7663c-114">ดู[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7663c-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


