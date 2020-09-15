---
title: สลับไซต์รากคลาสสิกของคุณด้วยไซต์ที่ทันสมัย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691198"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="4fbdd-102">สลับไซต์รากคลาสสิกของคุณด้วยไซต์ที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="4fbdd-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="4fbdd-103">ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน๒๐๑๙คุณสามารถเปลี่ยนไซต์รากของคุณไปยังไซต์ที่ทันสมัยได้โดยใช้ Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4fbdd-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="4fbdd-104">ถ้าคุณมีไซต์ที่แตกต่างกันที่คุณต้องการใช้เป็นไซต์รากของคุณคุณสามารถแทนที่ [(swap) ไซต์ราก](https://docs.microsoft.com/sharepoint/modern-root-site) ด้วยได้</span><span class="sxs-lookup"><span data-stu-id="4fbdd-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="4fbdd-105">ใช้ [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับตำแหน่งที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์ต้นฉบับ</span><span class="sxs-lookup"><span data-stu-id="4fbdd-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4fbdd-106">พร้อมใช้งานสำหรับไซต์ทีมทั้งสอง (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="4fbdd-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="4fbdd-107">ความสามารถเพิ่มเติมจะได้รับการแนะนำในเร็วๆนี้ที่จะช่วยให้คุณสามารถใช้เนื้อหาบนไซต์ได้แต่แปลงไซต์ที่มีอยู่แล้วไปยังไซต์การติดต่อสื่อสาร</span><span class="sxs-lookup"><span data-stu-id="4fbdd-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="4fbdd-108">ความสามารถเหล่านี้จะได้รับการรีดออกมาค่อยๆ</span><span class="sxs-lookup"><span data-stu-id="4fbdd-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="4fbdd-109">ดำเนินการตรวจสอบศูนย์ข้อความสำหรับการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="4fbdd-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4fbdd-110">ปัญหาที่ทราบเกี่ยวกับการสลับไซต์</span><span class="sxs-lookup"><span data-stu-id="4fbdd-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="4fbdd-111">ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="4fbdd-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4fbdd-112">เนื้อหาจะต้องถูก recrawled เพื่ออัปเดตดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="4fbdd-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4fbdd-113">ไม่จำเป็นต้องมีขั้นตอนด้วยตนเอง-สิ่งนี้จะถูกดำเนินการโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="4fbdd-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="4fbdd-114">สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "คงที่" (เช่นไฟล์การซิงค์และไฟล์ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="4fbdd-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4fbdd-115">ถ้าไซต์ต้นฉบับเป็นไซต์ข่าวสารขององค์กรให้อัปเดต URL</span><span class="sxs-lookup"><span data-stu-id="4fbdd-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="4fbdd-116">รับรายการของไซต์ข่าวสารขององค์กรทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="4fbdd-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="4fbdd-117">ไซต์ Project Server อาจจำเป็นต้องมีการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่าพวกเขายังคงเชื่อมโยงอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="4fbdd-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
