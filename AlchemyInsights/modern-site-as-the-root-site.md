---
title: สมัยใหม่ไซต์เป็นไซต์ราก
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057787"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="ba4c9-102">สมัยใหม่ไซต์เป็นไซต์ราก</span><span class="sxs-lookup"><span data-stu-id="ba4c9-102">Modern site as root site</span></span>

<span data-ttu-id="ba4c9-103">ลูกค้า[เป้าหมายย่อย](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)ในขณะนี้สามารถเปิดใช้งานประสบการณ์การใช้งานไซต์ของการสื่อสารแบบสมัยใหม่ที่ไซต์รากคลาสสิกของผู้เช่าของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="ba4c9-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="ba4c9-104">คุณลักษณะนี้สามารถเรียกใช้ โดยการเรียกใช้ cmdlet PowerShell แบบง่าย ๆ</span><span class="sxs-lookup"><span data-stu-id="ba4c9-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="ba4c9-105">ในการดำเนินการเสร็จสมบูรณ์ของ PowerShell command(s) ไซต์รากจะมีการสื่อสารไซต์โฮมเพจใหม่</span><span class="sxs-lookup"><span data-stu-id="ba4c9-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="ba4c9-106">รายละเอียดเกี่ยวกับ PowerShell cmdlet และคุณลักษณะความต้องการไม่มีอยู่ในบทความ[SPOCommSite เปิดใช้งาน](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="ba4c9-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="ba4c9-107">เราจะสามารถค่อย ๆ ย้อนนี้ออก ปิด โดยค่าเริ่มต้น ไปยังลูกค้าเป้าหมายย่อยใน 2019 พฤษภาคมล่วงหน้า และแบบโรออกจะใช้บริการทั่วโลก โดยจุดสิ้นสุดของเดือน 2019 มิถุนายน</span><span class="sxs-lookup"><span data-stu-id="ba4c9-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="ba4c9-108">ดำเนินต่อเพื่ออ้างอิงไปยัง[ศูนย์ข้อความ](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)สำหรับคุณลักษณะใหม่อื่น ๆ ด้วยแบบสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="ba4c9-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="ba4c9-109">**สิ่งสำคัญ**: อย่าลบไซต์รากคลาสสิกของการสร้างไซต์สื่อสารแบบสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="ba4c9-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="ba4c9-110">นี้จะไม่ได้รับการสนับสนุน โดย Microsoft</span><span class="sxs-lookup"><span data-stu-id="ba4c9-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="ba4c9-111">การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมด จนกว่าคุณคืนค่าไซต์ หรือสร้างไซต์ใหม่ที่ URL เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="ba4c9-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 