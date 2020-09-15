---
title: ไซต์ที่ทันสมัยเป็นไซต์ราก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666889"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="84347-102">ไซต์ที่ทันสมัยเป็นไซต์ราก</span><span class="sxs-lookup"><span data-stu-id="84347-102">Modern site as root site</span></span>

<span data-ttu-id="84347-103">เราได้เริ่มต้นใช้งานฟีเจอร์ใหม่ที่จะช่วยให้คุณสามารถ [สลับไซต์รากของไซต์แบบคลาสสิกของคุณกับไซต์ที่ทันสมัย](https://docs.microsoft.com/sharepoint/modern-root-site)ได้ไวร์</span><span class="sxs-lookup"><span data-stu-id="84347-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="84347-104">ใช้ [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับตำแหน่งที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์ต้นฉบับ</span><span class="sxs-lookup"><span data-stu-id="84347-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="84347-105">พร้อมใช้งานสำหรับไซต์ทีมทั้งสอง (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="84347-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="84347-106">อย่าลบไซต์รากคลาสสิกของคุณเพื่อสร้างไซต์การติดต่อสื่อสารที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="84347-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="84347-107">การทำเช่นนี้ไม่ได้รับการสนับสนุนโดยไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="84347-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="84347-108">การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมดได้จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="84347-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="84347-109">เราจะทำการสื่อสารฟีเจอร์นี้ผ่านทางศูนย์ข้อความ</span><span class="sxs-lookup"><span data-stu-id="84347-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="84347-110">คุณควรคาดหวังว่าฟีเจอร์นี้จะเปิดใช้งานในผู้เช่าของคุณในไม่ช้า</span><span class="sxs-lookup"><span data-stu-id="84347-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="84347-111">ปัญหาที่ทราบเกี่ยวกับการสลับไซต์</span><span class="sxs-lookup"><span data-stu-id="84347-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="84347-112">ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="84347-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="84347-113">เนื้อหาจะต้องถูก recrawled เพื่ออัปเดตดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="84347-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="84347-114">ไม่จำเป็นต้องมีขั้นตอนด้วยตนเองที่นี่การดำเนินการนี้จะดำเนินการโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="84347-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="84347-115">สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "คงที่" (เช่นไฟล์การซิงค์และไฟล์ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="84347-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="84347-116">ไซต์ Project Server อาจจำเป็นต้องมีการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่าพวกเขายังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="84347-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
