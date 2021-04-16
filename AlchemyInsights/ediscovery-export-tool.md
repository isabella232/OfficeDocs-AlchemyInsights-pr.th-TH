---
title: เครื่องมือส่งออก eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814607"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="1f61d-102">ไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery ได้ใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="1f61d-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="1f61d-103">ถ้าคุณไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery เพื่อดาวน์โหลดผลลัพธ์การค้นหา ให้ตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1f61d-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="1f61d-104">คอมพิวเตอร์ที่คุณใช้งานตรงตามเงื่อนไขต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1f61d-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="1f61d-105">Windows 7 และเวอร์ชันที่ใหม่กว่าเวอร์ชัน 32 บิตหรือ 64 บิต</span><span class="sxs-lookup"><span data-stu-id="1f61d-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="1f61d-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="1f61d-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="1f61d-107">เบราว์เซอร์ที่สนับสนุน:</span><span class="sxs-lookup"><span data-stu-id="1f61d-107">A supported browser:</span></span>

  - <span data-ttu-id="1f61d-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1f61d-108">Microsoft Edge</span></span>

    <span data-ttu-id="1f61d-109">หรือ</span><span class="sxs-lookup"><span data-stu-id="1f61d-109">Or</span></span>

  - <span data-ttu-id="1f61d-110">Internet Explorer 10 และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="1f61d-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="1f61d-111">เบราว์เซอร์อื่นๆ เช่น Google Chrome และ Mozilla Firefox ไม่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="1f61d-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="1f61d-112">องค์กรของคุณสามารถเชื่อมต่อกับจุดสิ้นสุดใน Azure ซึ่งเป็น **\* .blob.core.windows.net** (อักขระตัวแทนจะแสดงตัวระบุเฉพาะของงานส่งออกของคุณ)</span><span class="sxs-lookup"><span data-stu-id="1f61d-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="1f61d-113">คุณได้รับมอบหมายบทบาทส่งออกในศูนย์การปฏิบัติตามข้อบังคับด้านความปลอดภัยของ Microsoft 365 &amp;</span><span class="sxs-lookup"><span data-stu-id="1f61d-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="1f61d-114">ตามค่าเริ่มต้น บทบาทนี้จะถูกมอบหมายให้กับกลุ่มบทบาทตัวจัดการ eDiscovery เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="1f61d-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="1f61d-115">ดู[กําหนดสิทธิ์ eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="1f61d-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="1f61d-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="1f61d-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="1f61d-117">ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก: การส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า[100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="1f61d-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>