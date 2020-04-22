---
title: เว็บไซต์ที่ทันสมัยเป็นไซต์ราก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713810"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="ffbcf-102">ไซต์ที่ทันสมัยเป็นไซต์ราก</span><span class="sxs-lookup"><span data-stu-id="ffbcf-102">Modern site as root site</span></span>

<span data-ttu-id="ffbcf-103">เราได้เริ่มที่จะเปิดตัวคุณลักษณะใหม่ที่จะช่วยให้คุณ[แลกเปลี่ยนเว็บไซต์รากเว็บไซต์คลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="ffbcf-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="ffbcf-104">ใช้[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตําแหน่งของไซต์กับไซต์อื่นในขณะที่เก็บไซต์เดิม</span><span class="sxs-lookup"><span data-stu-id="ffbcf-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="ffbcf-105">พร้อมใช้งานสําหรับไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="ffbcf-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="ffbcf-106">อย่าลบไซต์รากของคุณคลาสสิกเพื่อสร้างไซต์การสื่อสารที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="ffbcf-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="ffbcf-107">ซึ่งไม่ได้รับการสนับสนุนโดย Microsoft</span><span class="sxs-lookup"><span data-stu-id="ffbcf-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="ffbcf-108">การลบไซต์รากจะทําให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงได้กับผู้ใช้ทุกคน จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="ffbcf-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="ffbcf-109">เราจะสื่อสารคุณลักษณะนี้ผ่านทางศูนย์ข้อความ</span><span class="sxs-lookup"><span data-stu-id="ffbcf-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="ffbcf-110">คุณควรคาดหวังว่าคุณลักษณะที่จะเปิดใช้งานในผู้เช่าของคุณในไม่ช้า</span><span class="sxs-lookup"><span data-stu-id="ffbcf-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="ffbcf-111">ปัญหาที่ทราบเกี่ยวกับการแลกเปลี่ยนไซต์</span><span class="sxs-lookup"><span data-stu-id="ffbcf-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="ffbcf-112">ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="ffbcf-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="ffbcf-113">เนื้อหาจะต้องถูกตระเวนใหม่เพื่อปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="ffbcf-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="ffbcf-114">ไม่มีขั้นตอนด้วยตนเองที่จําเป็นที่นี่, นี้จะกระทําโดยอัตโนมัติ.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="ffbcf-115">สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "แบบคงที่" (เช่น File Sync และไฟล์ OneNote) จะต้องถูกแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="ffbcf-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="ffbcf-116">ไซต์เซิร์ฟเวอร์โครงการอาจต้องถูกตรวจสอบเพื่อให้แน่ใจว่า พวกเขายังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="ffbcf-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
