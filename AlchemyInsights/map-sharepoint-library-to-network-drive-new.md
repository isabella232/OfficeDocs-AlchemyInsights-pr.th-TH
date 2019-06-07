---
title: แผนผังไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 7bb1f7d1b77ec5850109c9553ddfd894b3823946
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34754833"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="d4f37-102">แผนผังไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="d4f37-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="d4f37-103">ไลบรารีเป็นไดรฟ์เครือข่ายที่แมปเป็นแบบชั่วคราว และได้รับการสนับสนุน โดย Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="d4f37-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="d4f37-104">ในบางครั้งคุณต้องเปิดไซต์ SharePoint ใน Internet Explorer และเลือก "อยู่ลงชื่อเข้าใช้" เพื่อป้องกันไม่ให้เซสชันหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="d4f37-104">You must occasionally open the SharePoint site in Internet Explorer and select "Stay signed in" to prevent the session from expiring.</span></span> <span data-ttu-id="d4f37-105">แทน[ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>ซึ่งเป็น[แฟ้มตามความต้องการ](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)</span><span class="sxs-lookup"><span data-stu-id="d4f37-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="d4f37-106">เข้าถึงแฟ้มของคุณทั้งหมดใน OneDrive โดยไม่ต้องใช้เนื้อที่เก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="d4f37-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="d4f37-107">ถ้าคุณเลือกที่จะแมปไดร์ฟแทนการ[ใช้ไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ให้แน่ใจว่า คุณทำตามขั้นตอนต่าง ๆ ในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="d4f37-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="d4f37-108">**วิธีการตั้งค่าคอนฟิก และการแก้ไขปัญหาแมปไดรฟ์เครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="d4f37-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="d4f37-109">[ตั้งค่าคอนฟิก และการแก้ปัญหาแมปไดรฟ์เครือข่าย](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US)</span><span class="sxs-lookup"><span data-stu-id="d4f37-109">[Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="d4f37-110">หมายเหตุ: สำหรับ 10 Explorer อินเทอร์เน็ตกับ Windows 8 หรือ Windows 7 ที่ได้รับ "Access denied" หรือ "เส้นทางไม่สามารถเข้าถึงได้" เมื่อต้องการแมปไดรฟ์ ติดตั้งโปรแกรมแก้ไขด่วนนี้เพื่อแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="d4f37-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="d4f37-111">ไปที่[ข้อผิดพลาดเมื่อคุณเปิดไลบรารีเอกสาร SharePoint ใน Windows Explorer หรือแมปไดรฟ์เครือข่ายไปยังไลบรารีหลังจากที่คุณติดตั้ง Internet Explorer 10](https://support.microsoft.com/help/2846960)</span><span class="sxs-lookup"><span data-stu-id="d4f37-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>
