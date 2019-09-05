---
title: เว็บไซต์ที่ทันสมัยเป็นเว็บไซต์ราก
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753923"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="05d9c-102">เว็บไซต์ที่ทันสมัยเป็นเว็บไซต์ราก</span><span class="sxs-lookup"><span data-stu-id="05d9c-102">Modern site as root site</span></span>

<span data-ttu-id="05d9c-103">เราได้เริ่มที่จะเปิดตัวคุณลักษณะใหม่ที่จะช่วยให้คุณสามารถ[สลับเว็บไซต์รากเว็บไซต์คลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="05d9c-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="05d9c-104">ใช้[เรียก SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตำแหน่งที่ตั้งของไซต์ที่มีไซต์อื่นในขณะที่เก็บถาวรไซต์เดิม</span><span class="sxs-lookup"><span data-stu-id="05d9c-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="05d9c-105">พร้อมใช้งานสำหรับทั้งไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="05d9c-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="05d9c-106">อย่าลบไซต์รากคลาสสิกของคุณเพื่อสร้างไซต์การสื่อสารที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="05d9c-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="05d9c-107">นี้ไม่ได้รับการสนับสนุนโดย Microsoft</span><span class="sxs-lookup"><span data-stu-id="05d9c-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="05d9c-108">การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมดได้จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="05d9c-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="05d9c-109">เราจะสื่อสารคุณลักษณะนี้ผ่านทางศูนย์ข้อความ</span><span class="sxs-lookup"><span data-stu-id="05d9c-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="05d9c-110">คุณควรคาดหวังว่าคุณลักษณะนี้จะเปิดอยู่ในผู้เช่าของคุณในไม่ช้า</span><span class="sxs-lookup"><span data-stu-id="05d9c-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="05d9c-111">ปัญหาที่ทราบเกี่ยวกับการสลับเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="05d9c-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="05d9c-112">ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="05d9c-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="05d9c-113">เนื้อหาจะต้องมีการปรับปรุงดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="05d9c-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="05d9c-114">ไม่มีขั้นตอนที่กำหนดด้วยตนเองที่นี่จะทำโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="05d9c-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="05d9c-115">สิ่งใดก็ตามที่ขึ้นอยู่กับการเชื่อมโยง "คง" (เช่นแฟ้มซิงค์และแฟ้ม OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="05d9c-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="05d9c-116">ไซต์เซิร์ฟเวอร์โครงการอาจจำเป็นต้องตรวจสอบเพื่อให้แน่ใจว่าพวกเขายังคงเกี่ยวข้องอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="05d9c-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
