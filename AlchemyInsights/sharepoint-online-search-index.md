---
title: ค้นหาใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 85f29fabe3189fe248696155208b56d4901ab6de
ms.sourcegitcommit: b5370f0fc8da1e7e5ac960cb622a21612a9c86be
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/29/2020
ms.locfileid: "42341111"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="d12bf-102">การตระเวนเนื้อหาและการจัดทำดัชนีใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d12bf-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="d12bf-103">เนื้อหาต้องถูกตระเวนและเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้เพื่อค้นหาสิ่งที่พวกเขากำลังค้นหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d12bf-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="d12bf-104">ตรวจสอบให้แน่ใจว่าเนื้อหาสามารถพบได้โดยการ[ทำให้เนื้อหาไซต์ค้นหา](https://docs.microsoft.com/sharepoint/make-site-content-searchable)ได้</span><span class="sxs-lookup"><span data-stu-id="d12bf-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="d12bf-105">เมื่อคุณได้เปลี่ยนแปลงคุณสมบัติที่มีการจัดการหรือเมื่อคุณเปลี่ยนแปลงการแมปของคุณสมบัติที่ถูกตระเวนและมีการจัดการไซต์ต้องถูกตระเวนใหม่ก่อนที่การเปลี่ยนแปลงของคุณจะปรากฏในดัชนีการค้นหา</span><span class="sxs-lookup"><span data-stu-id="d12bf-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="d12bf-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ร้องขอการตระเวนด้วยตนเองและการจัดทำดัชนีใหม่ของไซต์ไลบรารีหรือรายการ](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="d12bf-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="d12bf-107">รออย่างน้อย24ชั่วโมงหลังจากร้องขอการตระเวนและดัชนีใหม่ทั้งหมดเพื่อดูว่าคุณยังคงประสบปัญหาหรือไม่</span><span class="sxs-lookup"><span data-stu-id="d12bf-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="d12bf-108">ถ้ามากกว่า24ชั่วโมงหลังจากที่คุณเริ่มต้นการตระเวนและดัชนีเต็มรูปแบบโปรดเข้าสู่ระบบกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="d12bf-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="d12bf-109">ในหลายกรณีเรากำลังหาทางแก้ไขปัญหาอยู่</span><span class="sxs-lookup"><span data-stu-id="d12bf-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d12bf-110">กรุณาให้เราอย่างน้อย24ชั่วโมงเพื่อให้การแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="d12bf-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="d12bf-111">**สิ่งสำคัญ**: ถ้าไซต์เอกสาร (ไลบรารี) หรือรายการถูกลบและยังคงแสดงอยู่ในผลลัพธ์การค้นหาผู้ใช้ควรได้รับ**ข้อผิดพลาด๔๐๔แฟ้มไม่พบ**เมื่อพยายามเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="d12bf-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="d12bf-112">ปัญหานี้ควรถูกบันทึกไว้เป็นกรณีการสนับสนุนสำหรับการตรวจสอบต่อไป</span><span class="sxs-lookup"><span data-stu-id="d12bf-112">This issue should be logged as a support case for further investigation.</span></span>



