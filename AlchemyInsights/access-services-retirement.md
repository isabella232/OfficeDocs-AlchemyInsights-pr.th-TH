---
title: ปลดเกษียณบริการเข้าถึง
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769483"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b3628-102">ปลดเกษียณบริการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="b3628-102">Access services retirement</span></span>

<span data-ttu-id="b3628-103">เมื่อเราประกาศใน MC97576 ในเดือน 2017 มีนาคม และดำเนินต่อเพื่อติดต่อสื่อสารผ่านปีผ่านมาตั้งแต่แรก Access Services จะถูกถอนจาก Office 365</span><span class="sxs-lookup"><span data-stu-id="b3628-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="b3628-104">ขั้นต่อไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูลเว็บการเข้าถึงที่ใช้รายการ SharePoint เป็นการจัดเก็บข้อมูลที่อยู่ภายใต้</span><span class="sxs-lookup"><span data-stu-id="b3628-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b3628-105">**วิธีไม่นี้ส่งผลต่อฉันอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="b3628-105">**How does this affect me?**</span></span>

<span data-ttu-id="b3628-106">เริ่มต้นเดือน 2019 มิถุนายน เราจะหยุดการสร้างฐานข้อมูลใหม่ของ Access ใน SharePoint แบบออนไลน์ และปิดบริการและโปรแกรมประยุกต์ใด ๆ ที่เหลือ โดย 2020 เมษายน</span><span class="sxs-lookup"><span data-stu-id="b3628-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b3628-107">**สิ่งที่ฉันต้องทำเพื่อเตรียมการสำหรับการเปลี่ยนแปลงนี้หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="b3628-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b3628-108">เราสนับสนุนให้คุณสามารถสร้างแผนการเปลี่ยนแปลงสำหรับฐานข้อมูลเว็บการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b3628-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="b3628-109">Admins สามารถใช้[สแกนเนอร์โปรแกรมประยุกต์ SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เมื่อต้องการรับสินค้าคงคลังของ apps Access ที่กำลังใช้ไซต์</span><span class="sxs-lookup"><span data-stu-id="b3628-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="b3628-110">มีหลายวิธีในการโยกย้ายข้อมูลจากฐานข้อมูล Access เว็บ:</span><span class="sxs-lookup"><span data-stu-id="b3628-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b3628-111">นำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือ ไปยังแฟ้ม Excel</span><span class="sxs-lookup"><span data-stu-id="b3628-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b3628-112">นอกจากนี้เรายังแนะนำสำรวจ Microsoft PowerApps เป็นแพลตฟอร์มตัวอื่นเพื่อสร้างการแก้ไขปัญหาทางธุรกิจไม่มีโค้ดสำหรับเว็บและอุปกรณ์มือถือ</span><span class="sxs-lookup"><span data-stu-id="b3628-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>