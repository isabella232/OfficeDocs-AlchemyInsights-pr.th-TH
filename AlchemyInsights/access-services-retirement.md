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
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050508"
---
# <a name="access-services-retirement"></a><span data-ttu-id="39789-102">การเข้าถึงบริการการเกษียณอายุ</span><span class="sxs-lookup"><span data-stu-id="39789-102">Access services retirement</span></span>

<span data-ttu-id="39789-103">ในขณะที่เราได้ประกาศใน MC97576 มีนาคม๒๐๑๗และยังคงสื่อสารในปีที่ผ่านมาบริการการเข้าถึงจะถูกตัดออกจาก Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="39789-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="39789-104">ขั้นตอนต่อไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูลการเข้าถึงเว็บที่ใช้รายการ SharePoint เป็นการจัดเก็บข้อมูลพื้นฐานของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="39789-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="39789-105">**วิธีนี้ส่งผลต่อฉันอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="39789-105">**How does this affect me?**</span></span>

<span data-ttu-id="39789-106">เริ่มตั้งแต่เดือนมิถุนายน๒๐๑๙เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint แบบออนไลน์และปิดบริการและแอปที่เหลืออยู่โดย๒๐๒๐เดือนเมษายน</span><span class="sxs-lookup"><span data-stu-id="39789-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="39789-107">**ฉันต้องทำอะไรเพื่อเตรียมความพร้อมสำหรับการเปลี่ยนแปลงนี้**</span><span class="sxs-lookup"><span data-stu-id="39789-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="39789-108">เราขอแนะนำให้คุณสร้างแผนการเปลี่ยนแปลงสำหรับฐานข้อมูลเว็บขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="39789-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="39789-109">ผู้ดูแลระบบสามารถใช้[สแกนเนอร์แอพลิเคชัน SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เพื่อขอรับสินค้าคงคลังของโปรแกรมประยุกต์ access ที่ไซต์กำลังใช้อยู่</span><span class="sxs-lookup"><span data-stu-id="39789-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="39789-110">มีหลายวิธีในการโยกย้ายข้อมูลในฐานข้อมูลเว็บของ Access:</span><span class="sxs-lookup"><span data-stu-id="39789-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="39789-111">การนำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือไปที่ไฟล์ Excel</span><span class="sxs-lookup"><span data-stu-id="39789-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="39789-112">นอกจากนี้เรายังแนะนำให้คุณสำรวจ Microsoft PowerApps เป็นแพลตฟอร์มอื่นเพื่อสร้างโซลูชันทางธุรกิจแบบไม่มีรหัสสำหรับเว็บและอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="39789-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>