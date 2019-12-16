---
title: ปัญหาการเชื่อมต่อของตัวออกแบบ SharePoint
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051732"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="8be4f-102">ปัญหาการเชื่อมต่อของตัวออกแบบ SharePoint</span><span class="sxs-lookup"><span data-stu-id="8be4f-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="8be4f-103">ถ้า SharePoint Designer กำลังประสบกับปัญหาการเชื่อมต่อไปยังไซต์ SharePoint โปรดลองใช้โซลูชันทั่วไปต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="8be4f-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="8be4f-104">ขั้นตอนที่ 1: ตรวจสอบว่า SharePoint Designer ๒๐๑๓ถูกปรับปรุงด้วยตัว[ออกแบบ Sharepoint Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)และ[2 สิงหาคม๒๐๑๖การปรับปรุงสำหรับ SharePoint Designer ๒๐๑๓](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="8be4f-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="8be4f-105">ขั้นตอนที่ 2: ล้างไฟล์แคชภายในเครื่อง:</span><span class="sxs-lookup"><span data-stu-id="8be4f-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="8be4f-106">ปิดตัวออกแบบ SharePoint ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="8be4f-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="8be4f-107">บนคอมพิวเตอร์เฉพาะที่ให้เอาแฟ้มทั้งหมดที่พบในแต่ละโฟลเดอร์ต่อไปนี้ออก</span><span class="sxs-lookup"><span data-stu-id="8be4f-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="8be4f-108">\ การขยายการเว็บเซิร์ฟเวอร์ \</span><span class="sxs-lookup"><span data-stu-id="8be4f-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="8be4f-109">\ '% \Nat\ \ ' \</span><span class="sxs-lookup"><span data-stu-id="8be4f-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="8be4f-110">\Napa\nater\ \</span><span class="sxs-lookup"><span data-stu-id="8be4f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="8be4f-111">เปิด SharePoint Designer ๒๐๑๓และป้อนบัญชีอีกครั้งเพื่อดูว่าการทำงานหรือไม่</span><span class="sxs-lookup"><span data-stu-id="8be4f-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="8be4f-112">ขั้นตอนที่ 3:[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="8be4f-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="8be4f-113">ขั้นตอนที่ 4: ผู้ดูแลระบบจะต้อง**อนุญาตให้สคริปต์ที่กำหนดเอง**ในการตั้งค่าศูนย์ดูแล sharepoint เพื่ออนุญาตให้มีการเชื่อมต่อ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="8be4f-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="8be4f-114">โปรดดูที่[อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="8be4f-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


