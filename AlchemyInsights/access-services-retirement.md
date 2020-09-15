---
title: การปลดเกษียณบริการเข้าถึง
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698701"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b312f-102">การปลดเกษียณบริการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="b312f-102">Access services retirement</span></span>

<span data-ttu-id="b312f-103">ในขณะที่เราได้ประกาศใน MC97576 ในเดือนมีนาคม๒๐๑๗และยังคงสื่อสารผ่านทางบริการการเข้าถึงปีที่ผ่านมาจะถูกถอนออกไป</span><span class="sxs-lookup"><span data-stu-id="b312f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="b312f-104">ขั้นตอนถัดไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูล Access บนเว็บที่ใช้รายการ SharePoint เป็นที่เก็บข้อมูลที่อยู่ภายใต้</span><span class="sxs-lookup"><span data-stu-id="b312f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b312f-105">**สิ่งนี้มีผลต่อฉันอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="b312f-105">**How does this affect me?**</span></span>

<span data-ttu-id="b312f-106">เริ่มต้นเดือนมิถุนายน๒๐๑๙เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint Online และปิดบริการและแอปพลิเคชันที่เหลือในเดือนเมษายน๒๐๒๐</span><span class="sxs-lookup"><span data-stu-id="b312f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b312f-107">**ฉันต้องทำอะไรบ้างเพื่อเตรียมพร้อมสำหรับการเปลี่ยนแปลงนี้**</span><span class="sxs-lookup"><span data-stu-id="b312f-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b312f-108">เราขอแนะนำให้คุณสร้างแผนการเปลี่ยนสำหรับฐานข้อมูล Access บนเว็บขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b312f-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="b312f-109">ผู้ดูแลระบบสามารถใช้ [สแกนเนอร์ของแอป SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) เพื่อขอรับสินค้าคงคลังของแอป access ที่ไซต์กำลังใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="b312f-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b312f-110">มีหลายวิธีในการโยกย้ายข้อมูลฐานข้อมูลบนเว็บของ Access:</span><span class="sxs-lookup"><span data-stu-id="b312f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b312f-111">การนำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือไปยังไฟล์ Excel</span><span class="sxs-lookup"><span data-stu-id="b312f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b312f-112">นอกจากนี้เรายังแนะนำให้สำรวจ Microsoft PowerApps เป็นแพลตฟอร์มสำหรับการสร้างโซลูชันทางธุรกิจสำหรับเว็บและอุปกรณ์เคลื่อนที่ไม่ใช่โค้ด</span><span class="sxs-lookup"><span data-stu-id="b312f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>