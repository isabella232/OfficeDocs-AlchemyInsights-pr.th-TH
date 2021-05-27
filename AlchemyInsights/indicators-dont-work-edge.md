---
title: ตัวบ่งชี้ไม่ใช้งานโดยใช้เบราว์เซอร์ Microsoft Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676469"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="98721-102">ตัวบ่งชี้ไม่ใช้งานโดยใช้เบราว์เซอร์ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="98721-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="98721-103">หลังจากที่คุณสร้างตัวบ่งชี้ Edge (SmartScreen) จะไม่แสดงขึ้น</span><span class="sxs-lookup"><span data-stu-id="98721-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="98721-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="98721-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="98721-105">ขั้นตอนที่ 1: ตรวจสอบให้แน่ใจว่า</span><span class="sxs-lookup"><span data-stu-id="98721-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="98721-106">ตรวจสอบว่าตัวบ่งชี้ถูกต้อง (ไม่มีการพิมพ์ผิดใน IP/URL การปฏิบัติการที่ถูกต้อง กลุ่ม RBAC ที่ถูกต้อง)</span><span class="sxs-lookup"><span data-stu-id="98721-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="98721-107">รออย่างน้อย 2 ชั่วโมงหลังจากสร้างตัวบ่งชี้เพื่อใช้เวลาในการเวลาแฝงที่เป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="98721-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="98721-108">ยืนยันว่าระบบออนบอร์ดกับ Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="98721-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="98721-109">ตรวจสอบว่าระบบนั้นสามารถสื่อสารกับระบบคลาวด์ได้</span><span class="sxs-lookup"><span data-stu-id="98721-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="98721-110">ตรวจสอบว่า SmartScreen เปิดใช้งานและเข้าถึงได้โดย [ไปที่ไซต์](https://demo.smartscreen.msft.net)ทดสอบ</span><span class="sxs-lookup"><span data-stu-id="98721-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="98721-111">ขั้นตอนที่ 2: แก้ไขปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="98721-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="98721-112">ตรวจสอบให้แน่ใจว่าไคลเอ็นต์ตรงตามความต้องการ</span><span class="sxs-lookup"><span data-stu-id="98721-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="98721-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="98721-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="98721-114">ตรวจสอบให้แน่ใจว่าคุณใช้เบราว์เซอร์ Microsoft Edge เวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="98721-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="98721-115">เมื่อต้องการค้นหาเวอร์ชันล่าสุด ให้ดู[ค้นหาเวอร์ชันMicrosoft Edgeเวอร์ชัน](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)ที่คุณมี</span><span class="sxs-lookup"><span data-stu-id="98721-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="98721-116">รีสตาร์ตเบราว์เซอร์ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="98721-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="98721-117">นําทางไปยังไซต์ที่คุณได้ตั้งค่าตัวบ่งชี้ไว้</span><span class="sxs-lookup"><span data-stu-id="98721-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="98721-118">ถ้าไซต์ไม่ปรากฏตามที่คาดไว้ ให้ไปยังขั้นตอนที่ 3</span><span class="sxs-lookup"><span data-stu-id="98721-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="98721-119">ขั้นตอนที่ 3: รวบรวมข้อมูล</span><span class="sxs-lookup"><span data-stu-id="98721-119">Step 3: Collect data</span></span>

- <span data-ttu-id="98721-120">รวบรวมข้อมูล **การวินิจฉัย MDEClientAnalyzer**</span><span class="sxs-lookup"><span data-stu-id="98721-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="98721-121">ดูคําแนะ[นําที่ ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoint](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="98721-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="98721-122">ถ้าคุณคุ้นเคยกับการติดตั้งและการรวบรวมการติดตาม Fiddler ให้ดู[Telerik Fiddler](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="98721-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="98721-123">ถ้าคุณต้องการแนวทางจากฝ่ายสนับสนุนของ Microsoft ให้เลือกไอคอน การสนับสนุน ทางด้านล่างเพื่อเปิดกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="98721-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
