---
title: เครื่องมือส่งออก eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277920"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="1e71c-102">ไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery ได้ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1e71c-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="1e71c-103">ถ้าคุณไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery เพื่อดาวน์โหลดผลลัพธ์การค้นหาให้ตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1e71c-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="1e71c-104">คอมพิวเตอร์ที่คุณกำลังใช้ตรงกับ requisites เหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="1e71c-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="1e71c-105">Windows 7 เวอร์ชัน๓๒หรือ๖๔บิตและเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="1e71c-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="1e71c-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="1e71c-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="1e71c-107">เบราว์เซอร์ที่ได้รับการสนับสนุน:</span><span class="sxs-lookup"><span data-stu-id="1e71c-107">A supported browser:</span></span>

  - <span data-ttu-id="1e71c-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1e71c-108">Microsoft Edge</span></span>

    <span data-ttu-id="1e71c-109">หรือ</span><span class="sxs-lookup"><span data-stu-id="1e71c-109">Or</span></span>

  - <span data-ttu-id="1e71c-110">Internet Explorer 10 และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="1e71c-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="1e71c-111">เบราว์เซอร์อื่นๆเช่น Google Chrome และ Mozilla Firefox จะไม่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="1e71c-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="1e71c-112">องค์กรของคุณสามารถเชื่อมต่อกับจุดสิ้นสุดใน Azure ซึ่งเป็น\*\* \* blob.core.windows.net\*\* (อักขระตัวแทนจะแสดงตัวระบุที่ไม่ซ้ำกันสำหรับงานส่งออกของคุณ)</span><span class="sxs-lookup"><span data-stu-id="1e71c-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="1e71c-113">คุณได้รับมอบหมายบทบาทการส่งออกใน &amp; ศูนย์การปฏิบัติตามนโยบายด้านความปลอดภัยของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="1e71c-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="1e71c-114">ตามค่าเริ่มต้นบทบาทนี้จะได้รับการกำหนดให้กับกลุ่มบทบาทผู้จัดการ eDiscovery เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="1e71c-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="1e71c-115">ให้ดูที่[กำหนดสิทธิ์ eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="1e71c-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="1e71c-116">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ส่งออกผลลัพธ์การค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="1e71c-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="1e71c-117">ถ้าคุณกำลังส่งออกกล่องจดหมายมากกว่า100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก:[ส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="1e71c-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>