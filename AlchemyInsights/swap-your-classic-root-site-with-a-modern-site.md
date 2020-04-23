---
title: สลับเว็บไซต์รากคลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741563"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="34986-102">สลับเว็บไซต์รากคลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="34986-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="34986-103">ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน 2019 คุณสามารถเปลี่ยนไซต์รากของคุณเป็นไซต์ที่ทันสมัย โดยใช้ Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="34986-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="34986-104">หากคุณมีเว็บไซต์อื่นที่คุณต้องการใช้เป็นไซต์รากของคุณคุณสามารถแทนที่[(swap) ไซต์ราก](https://docs.microsoft.com/sharepoint/modern-root-site)กับมัน</span><span class="sxs-lookup"><span data-stu-id="34986-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="34986-105">ใช้[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตําแหน่งของไซต์กับไซต์อื่นในขณะที่เก็บไซต์เดิม</span><span class="sxs-lookup"><span data-stu-id="34986-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="34986-106">พร้อมใช้งานสําหรับไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="34986-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="34986-107">ความสามารถเพิ่มเติมจะถูกนํามาใช้ในเร็ว ๆ นี้ที่จะช่วยให้คุณเพื่อให้การใช้เนื้อหาในเว็บไซต์ แต่แปลงเว็บไซต์ที่มีอยู่ไปยังไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="34986-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="34986-108">ความสามารถเหล่านี้จะถูกรีดออกค่อยๆ</span><span class="sxs-lookup"><span data-stu-id="34986-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="34986-109">ตรวจสอบการปรับปรุงศูนย์ข้อความต่อไป</span><span class="sxs-lookup"><span data-stu-id="34986-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="34986-110">ปัญหาที่ทราบเกี่ยวกับการแลกเปลี่ยนไซต์</span><span class="sxs-lookup"><span data-stu-id="34986-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="34986-111">ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="34986-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="34986-112">เนื้อหาจะต้องถูกตระเวนใหม่เพื่อปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="34986-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="34986-113">ไม่มีขั้นตอนด้วยตนเองที่จําเป็น - นี้จะทําโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="34986-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="34986-114">สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "แบบคงที่" (เช่น File Sync และไฟล์ OneNote) จะต้องถูกแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="34986-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="34986-115">ถ้าไซต์ต้นทางเป็นไซต์ข่าวสารขององค์กร ให้อัปเดต URL</span><span class="sxs-lookup"><span data-stu-id="34986-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="34986-116">ดูรายการไซต์ข่าวสารขององค์กรทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="34986-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="34986-117">ไซต์เซิร์ฟเวอร์โครงการอาจต้องถูกตรวจสอบเพื่อให้แน่ใจว่า พวกเขายังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="34986-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
