---
title: ค้นหาใน SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770786"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="89416-102">การรวบรวมเนื้อหาและการทำดัชนีใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="89416-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="89416-103">เนื้อหาต้องถูกตระเวนและเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้เพื่อค้นหาสิ่งที่พวกเขากำลังค้นหาใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="89416-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="89416-104">ตรวจสอบให้แน่ใจว่าสามารถค้นหาเนื้อหาได้โดยการทำให้เนื้อหาของ [ไซต์สามารถค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable)ได้</span><span class="sxs-lookup"><span data-stu-id="89416-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="89416-105">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการหรือเมื่อคุณเปลี่ยนแปลงการแมปของคุณสมบัติที่ตระเวนและที่มีการจัดการแล้วไซต์จะต้องถูกตระเวนใหม่ก่อนที่การเปลี่ยนแปลงของคุณจะปรากฏในดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="89416-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="89416-106">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การร้องขอการตระเวนและการทำดัชนีของไซต์ใหม่ด้วยตนเองไลบรารีหรือรายการ](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="89416-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="89416-107">รออย่างน้อย24ชั่วโมงหลังจากร้องขอการตระเวนและดัชนีทั้งหมดด้วยตนเองเพื่อดูว่าคุณยังพบปัญหาอยู่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="89416-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="89416-108">ถ้ามีการส่งผ่าน24ชั่วโมงหลังจากที่คุณเริ่มต้นการตระเวนและการทำดัชนีแบบเต็มแล้วโปรดเข้าสู่ระบบกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="89416-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="89416-109">ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="89416-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="89416-110">โปรดแจ้งให้เราทราบอย่างน้อย24ชั่วโมงเพื่อให้โซลูชันเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="89416-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="89416-111">**สิ่งสำคัญ**: ถ้าไซต์เอกสาร (ไลบรารี) หรือรายการถูกลบและยังคงแสดงอยู่ในผลลัพธ์การค้นหาผู้ใช้จะได้รับ **ไฟล์๔๐๔ข้อผิดพลาดไม่พบ** เมื่อพยายามเข้าถึงไฟล์นั้น</span><span class="sxs-lookup"><span data-stu-id="89416-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="89416-112">ปัญหานี้ควรถูกบันทึกเป็นกรณีสนับสนุนสำหรับการตรวจสอบเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="89416-112">This issue should be logged as a support case for further investigation.</span></span>



