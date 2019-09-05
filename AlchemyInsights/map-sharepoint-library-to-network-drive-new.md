---
title: แมปไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: c7b16cb448684d3f68be84fda4d9de201b953ffb
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734904"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="a3b67-102">แมปไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="a3b67-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="a3b67-103">การแมปไลบรารีเป็นไดรฟ์เครือข่ายเป็นแบบถาวรและได้รับการสนับสนุนผ่านทาง Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="a3b67-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="a3b67-104">คุณต้องเปิดไซต์ SharePoint ใน Internet Explorer เป็นครั้งคราวและเลือก**ลงชื่อ**เข้าใช้เพื่อป้องกันไม่ให้เซสชันหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="a3b67-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="a3b67-105">ให้</a> [ซิงค์แฟ้ม SharePoint กับไคลเอ็นต์ซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ซึ่งมี[แฟ้มตามความต้อง](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)การแทน</span><span class="sxs-lookup"><span data-stu-id="a3b67-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="a3b67-106">เข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive โดยไม่ต้องใช้พื้นที่จัดเก็บข้อมูลภายใน</span><span class="sxs-lookup"><span data-stu-id="a3b67-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="a3b67-107">ถ้าคุณเลือกที่จะแมปไดรฟ์แทนการ[ใช้ไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ให้แน่ใจว่าคุณทำตามขั้นตอนในบทความด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="a3b67-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="a3b67-108">**วิธีการกำหนดค่าและแก้ไขปัญหาไดรฟ์เครือข่ายที่แมป**</span><span class="sxs-lookup"><span data-stu-id="a3b67-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="a3b67-109">ดู[ที่การแก้ไขปัญหาไดรฟ์เครือข่ายที่ถูกแมปที่เชื่อมต่อกับ SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="a3b67-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="a3b67-110">หมายเหตุ: ถ้าคุณใช้ Internet Explorer 10 กับ Windows 8 หรือ Windows 7 และได้รับการ**ปฏิเสธการเข้าถึง**หรือ**เส้นทางไม่สามารถเข้าถึง**ได้เมื่อทำการแมปไดรฟ์ให้ติดตั้ง[โปรแกรมแก้ไขด่วนนี้](https://support.microsoft.com/help/2846960)เพื่อแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="a3b67-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
