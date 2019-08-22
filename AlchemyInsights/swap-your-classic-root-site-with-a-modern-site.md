---
title: สลับไซต์รากของคุณแบบคลาสสิคกับไซต์สมัยใหม่
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501098"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="84f19-102">สลับไซต์รากของคุณแบบคลาสสิคกับไซต์สมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="84f19-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="84f19-103">ถ้าระบบของคุณถูกตั้งค่าไว้ก่อน 2019 เมษายน คุณสามารถเปลี่ยนไซต์รากของคุณไปยังไซต์สมัยใหม่ โดยใช้ Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="84f19-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="84f19-104">ถ้าคุณมีไซต์อื่นที่คุณต้องการใช้เป็นไซต์รากของคุณ คุณสามารถแทน (สลับ) รากไซต์ดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="84f19-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="84f19-105">ใช้[Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)การสลับตำแหน่งของไซต์ที่มีไซต์อื่นในขณะที่เก็บถาวรไซต์ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="84f19-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="84f19-106">พร้อมใช้งานสำหรับทั้งไซต์สำหรับทีม (ไม่ได้เชื่อมต่อไปยังกลุ่ม) และไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="84f19-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="84f19-107">ความสามารถเพิ่มเติมจะถูกนำมาใช้ในไม่ช้า ที่จะช่วยให้คุณสามารถเก็บโดยใช้เนื้อหาบนไซต์ แต่แปลงในไซต์ที่มีอยู่ไปยังไซต์สื่อสาร</span><span class="sxs-lookup"><span data-stu-id="84f19-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="84f19-108">ความสามารถเหล่านี้จะสามารถย้อนออกทีละน้อย</span><span class="sxs-lookup"><span data-stu-id="84f19-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="84f19-109">ดำเนินการตรวจสอบศูนย์ Office 365 ข้อความสำหรับการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="84f19-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="84f19-110">ปัญหาที่ทราบ ด้วยการเปลี่ยนไซต์</span><span class="sxs-lookup"><span data-stu-id="84f19-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="84f19-111">ไซต์ปลายทางอาจส่งคืน (HTTP 404) เกิดข้อผิดพลาด "ไม่พบ" ในระยะเวลาสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="84f19-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="84f19-112">เนื้อหาจะต้องมี recrawled ในการปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="84f19-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="84f19-113">ไม่มีขั้นตอนด้วยตนเองที่จำเป็น - จะทำสิ่งนี้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="84f19-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="84f19-114">สิ่งใดขึ้นอยู่กับการเชื่อมโยง "คง" (เช่นแฟ้มที่ซิงค์แฟ้มและ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="84f19-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="84f19-115">หากไซต์ต้นทางไซต์ที่มีข่าวสารขององค์กร ปรับปรุง URL</span><span class="sxs-lookup"><span data-stu-id="84f19-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="84f19-116">ดูรายการไซต์ข่าวสารขององค์กรทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="84f19-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="84f19-117">ไซต์เซิร์ฟเวอร์โครงการอาจจำเป็นจะต้องตรวจสอบเพื่อให้มั่นใจว่า จะยังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="84f19-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





