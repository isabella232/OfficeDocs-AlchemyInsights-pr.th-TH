---
title: คลังซอฟต์แวร์หายไปหรือไม่ความไม่ถูกต้อง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676517"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="f8fd3-102">คลังซอฟต์แวร์หายไปหรือไม่ความไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f8fd3-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="f8fd3-103">คลังซอฟต์แวร์ใน การจัดการภัยคุกคามและช่องโหว่ (TVM) คือรายการซอฟต์แวร์ที่รู้จักในองค์กรของคุณที่มีการแจงนับแพลตฟอร์มทั่วไป (CPE) อย่างเป็นทางการ</span><span class="sxs-lookup"><span data-stu-id="f8fd3-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="f8fd3-104">ผลิตภัณฑ์ซอฟต์แวร์ที่ไม่มี CPE อย่างเป็นทางการไม่มีช่องโหว่ที่เผยแพร่</span><span class="sxs-lookup"><span data-stu-id="f8fd3-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="f8fd3-105">สินค้าคงคลังยังมีรายละเอียด เช่น ชื่อของผู้ขาย จํานวนของผู้โฆษณา ภัยคุกคาม และจํานวนอุปกรณ์ที่ถูกแสดง</span><span class="sxs-lookup"><span data-stu-id="f8fd3-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="f8fd3-106">การเปลี่ยนแปลงซอฟต์แวร์บนอุปกรณ์มักจะแสดงในพอร์ทัลความปลอดภัยภายในสองชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="f8fd3-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="f8fd3-107">อย่างไรก็ตาม บางครั้งอาจใช้เวลานานกว่านั้น</span><span class="sxs-lookup"><span data-stu-id="f8fd3-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="f8fd3-108">ขณะนี้ยังไม่มีวิธีบังคับซิงค์ นี่คือแบบประเมินอย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="f8fd3-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="f8fd3-109">ถ้าคุณเปลี่ยนแปลงซอฟต์แวร์ และการเปลี่ยนแปลงใน TVM ไม่ถูกต้องหลังจากผ่านไป 5 ชั่วโมง ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f8fd3-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="f8fd3-110">ตรวจสอบส่วนหลักฐานซอฟต์แวร์เพื่อเข้าใจว่าซอฟต์แวร์ถูกตรวจพบอย่างไร</span><span class="sxs-lookup"><span data-stu-id="f8fd3-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="f8fd3-111">ตรวจสอบให้แน่ใจว่าซอฟต์แวร์ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="f8fd3-111">Make sure that the software is supported.</span></span> <span data-ttu-id="f8fd3-112">ซอฟต์แวร์อาจมองเห็นได้ที่ระดับอุปกรณ์เท่านั้น แม้ว่าซอฟต์แวร์ดังกล่าวไม่ได้รับการสนับสนุนการจัดการภัยคุกคามและช่องโหว่อยู่</span><span class="sxs-lookup"><span data-stu-id="f8fd3-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="f8fd3-113">อย่างไรก็ตาม มีเฉพาะข้อมูลที่จํากัดเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f8fd3-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="f8fd3-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="f8fd3-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="f8fd3-115">**หมายเหตุ**: การรายงานความแม่นยําจากพอร์ทัล MDE คือช่องทางแบบทางเดียวสู่ทางวิศวกรรม</span><span class="sxs-lookup"><span data-stu-id="f8fd3-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="f8fd3-116">หากปัญหาเร่งด่วน ให้เปิดตั๋วการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="f8fd3-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="f8fd3-117">For more information, see [Software inventory - การจัดการภัยคุกคามและช่องโหว่](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="f8fd3-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>