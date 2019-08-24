---
title: สมัยใหม่ไซต์เป็นไซต์ราก
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620778"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="b2b75-102">สมัยใหม่ไซต์เป็นไซต์ราก</span><span class="sxs-lookup"><span data-stu-id="b2b75-102">Modern site as root site</span></span>

<span data-ttu-id="b2b75-103">เราได้เริ่มไวร์คุณลักษณะใหม่ที่จะอนุญาตให้คุณสลับไซต์รากของไซต์คลาสสิกกับไซต์สมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="b2b75-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="b2b75-104">ใช้[Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)การสลับตำแหน่งของไซต์ที่มีไซต์อื่นในขณะที่เก็บถาวรไซต์ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="b2b75-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b2b75-105">พร้อมใช้งานสำหรับทั้งไซต์สำหรับทีม (ไม่ได้เชื่อมต่อไปยังกลุ่ม) และไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="b2b75-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="b2b75-106">ลบไซต์รากคลาสสิกของการสร้างไซต์สื่อสารแบบสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="b2b75-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="b2b75-107">นี้จะไม่ได้รับการสนับสนุน โดย Microsoft</span><span class="sxs-lookup"><span data-stu-id="b2b75-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="b2b75-108">การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมด จนกว่าคุณคืนค่าไซต์ หรือสร้างไซต์ใหม่ที่ URL เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="b2b75-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="b2b75-109">เราจะสื่อสารคุณลักษณะนี้ผ่านทางข้อความกึ่งกลาง</span><span class="sxs-lookup"><span data-stu-id="b2b75-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="b2b75-110">คุณควรคาดหวังคุณลักษณะต้องการในการเช่าของคุณในไม่ช้า</span><span class="sxs-lookup"><span data-stu-id="b2b75-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b2b75-111">ปัญหาที่ทราบ ด้วยการเปลี่ยนไซต์</span><span class="sxs-lookup"><span data-stu-id="b2b75-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="b2b75-112">ไซต์ปลายทางอาจส่งคืน (HTTP 404) เกิดข้อผิดพลาด "ไม่พบ" ในระยะเวลาสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="b2b75-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b2b75-113">เนื้อหาจะต้องมี recrawled ในการปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="b2b75-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b2b75-114">ขั้นตอนการด้วยตนเองไม่จำเป็นต้องใช้ที่นี่ จะทำสิ่งนี้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b2b75-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="b2b75-115">สิ่งใดขึ้นอยู่กับการเชื่อมโยง "คง" (เช่นแฟ้มที่ซิงค์แฟ้มและ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="b2b75-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b2b75-116">ไซต์เซิร์ฟเวอร์โครงการอาจจำเป็นจะต้องตรวจสอบเพื่อให้มั่นใจว่า จะยังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b2b75-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
