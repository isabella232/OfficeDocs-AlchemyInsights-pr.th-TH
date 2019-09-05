---
title: สลับเว็บไซต์รากคลาสสิกของคุณด้วยเว็บไซต์ที่ทันสมัย
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749279"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="1e370-102">สลับเว็บไซต์รากคลาสสิกของคุณด้วยเว็บไซต์ที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="1e370-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="1e370-103">ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน๒๐๑๙คุณสามารถเปลี่ยนไซต์รากของคุณไปยังไซต์ที่ทันสมัยโดยใช้ Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1e370-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="1e370-104">ถ้าคุณมีเว็บไซต์อื่นที่คุณต้องการใช้เป็นไซต์รากของคุณคุณสามารถแทน[ที่ (สลับ) ไซต์ราก](https://docs.microsoft.com/sharepoint/modern-root-site)กับมัน</span><span class="sxs-lookup"><span data-stu-id="1e370-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="1e370-105">ใช้[เรียก SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตำแหน่งที่ตั้งของไซต์ที่มีไซต์อื่นในขณะที่เก็บถาวรไซต์เดิม</span><span class="sxs-lookup"><span data-stu-id="1e370-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1e370-106">พร้อมใช้งานสำหรับทั้งไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="1e370-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="1e370-107">ความสามารถเพิ่มเติมจะได้รับการแนะนำในเร็วๆนี้ที่จะช่วยให้คุณสามารถใช้เนื้อหาบนเว็บไซต์แต่แปลงเว็บไซต์ที่มีอยู่ไปยังไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="1e370-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="1e370-108">ความสามารถเหล่านี้จะทยอยออกมาเรื่อยๆ</span><span class="sxs-lookup"><span data-stu-id="1e370-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="1e370-109">ดำเนินการตรวจสอบศูนย์ข้อความของ Office ๓๖๕สำหรับการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="1e370-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1e370-110">ปัญหาที่ทราบเกี่ยวกับการสลับเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="1e370-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="1e370-111">ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="1e370-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1e370-112">เนื้อหาจะต้องมีการปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="1e370-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1e370-113">ไม่มีขั้นตอนที่จำเป็นด้วยตนเอง-นี้จะทำโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1e370-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="1e370-114">สิ่งใดก็ตามที่ขึ้นอยู่กับการเชื่อมโยง "คง" (เช่นแฟ้มซิงค์และแฟ้ม OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="1e370-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1e370-115">ถ้าไซต์ต้นทางเป็นไซต์ข่าวสารขององค์กรให้ปรับปรุง URL</span><span class="sxs-lookup"><span data-stu-id="1e370-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="1e370-116">ดูรายชื่อไซต์ข่าวสารขององค์กรทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="1e370-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="1e370-117">ไซต์เซิร์ฟเวอร์โครงการอาจจำเป็นต้องตรวจสอบเพื่อให้แน่ใจว่าพวกเขายังคงเกี่ยวข้องอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1e370-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





