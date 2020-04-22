---
title: การเข้าถึงบริการการเกษียณอายุ
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687277"
---
# <a name="access-services-retirement"></a><span data-ttu-id="098c7-102">การเข้าถึงบริการการเกษียณอายุ</span><span class="sxs-lookup"><span data-stu-id="098c7-102">Access services retirement</span></span>

<span data-ttu-id="098c7-103">ในเดือนมีนาคม 2017 และยังคงสื่อสารกันอย่างต่อเนื่องตลอดปีที่ผ่านมา</span><span class="sxs-lookup"><span data-stu-id="098c7-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="098c7-104">ขั้นตอนถัดไปในกระบวนการนี้จะเป็นการเอาฐานข้อมูล Access Web ที่ใช้รายการ SharePoint เป็นที่เก็บข้อมูลต้นแบบออก</span><span class="sxs-lookup"><span data-stu-id="098c7-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="098c7-105">**สิ่งนี้ส่งผลต่อฉันอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="098c7-105">**How does this affect me?**</span></span>

<span data-ttu-id="098c7-106">เริ่ม 2019 มิถุนายน เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint Online และปิดบริการและแอปที่เหลือภายในเดือนเมษายน 2020</span><span class="sxs-lookup"><span data-stu-id="098c7-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="098c7-107">**ฉันต้องทําอะไรบ้างเพื่อเตรียมการเปลี่ยนแปลงนี้**</span><span class="sxs-lookup"><span data-stu-id="098c7-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="098c7-108">เราสนับสนุนให้คุณสร้างแผนการเปลี่ยนสําหรับฐานข้อมูลเว็บ Access ขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="098c7-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="098c7-109">ผู้ดูแลระบบสามารถใช้[โปรแกรมสแกนโปรแกรมประยุกต์ SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เพื่อขอรับสินค้าคงคลังของโปรแกรมประยุกต์ Access ที่ไซต์กําลังใช้อยู่</span><span class="sxs-lookup"><span data-stu-id="098c7-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="098c7-110">มีหลายวิธีในการย้ายข้อมูลฐานข้อมูลเว็บ Access:</span><span class="sxs-lookup"><span data-stu-id="098c7-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="098c7-111">การนําเข้าฐานข้อมูล Access ภายในเครื่อง (.AS) ACCDB) หรือไปยังไฟล์ Excel</span><span class="sxs-lookup"><span data-stu-id="098c7-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="098c7-112">เราขอแนะนําให้สํารวจ Microsoft PowerApps เป็นแพลตฟอร์มอื่นเพื่อสร้างโซลูชันทางธุรกิจที่ไม่มีรหัสสําหรับเว็บและโทรศัพท์มือถือ</span><span class="sxs-lookup"><span data-stu-id="098c7-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>