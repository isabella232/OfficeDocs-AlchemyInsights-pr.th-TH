---
title: กฎการลดพื้นหน้าของการโจมตี
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676445"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="e24d7-102">กฎการลดพื้นหน้าของการโจมตี</span><span class="sxs-lookup"><span data-stu-id="e24d7-102">Attack surface reduction rules</span></span>

<span data-ttu-id="e24d7-103">การยกเว้นไฟล์หรือโฟลเดอร์อาจลดการป้องกันอย่างร้ายแรงจากกฎการลดพื้นหน้าของการโจมตีได้</span><span class="sxs-lookup"><span data-stu-id="e24d7-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="e24d7-104">ไฟล์ที่ถูกบล็อกโดยกฎจะได้รับอนุญาตให้เรียกใช้ และจะไม่มีบันทึกรายงานหรือเหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="e24d7-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="e24d7-105">การยกเว้นจะใช้กับกฎทั้งหมดที่อนุญาตให้ยกเว้นได้</span><span class="sxs-lookup"><span data-stu-id="e24d7-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="e24d7-106">การยกเว้น ASR จะใช้ไวยากรณ์เดียวกับโปรแกรมป้องกันไวรัสของ Microsoft Defenderแยกออก</span><span class="sxs-lookup"><span data-stu-id="e24d7-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="e24d7-107">For details, see [Configure and validate exclusions for โปรแกรมป้องกันไวรัสของ Microsoft Defender scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="e24d7-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="e24d7-108">เพื่อหลีกเลี่ยงปัญหา ให้ตรวจดู[ข้อผิดพลาดทั่วไปเพื่อหลีกเลี่ยงเมื่อระบุข้อยกเว้น](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="e24d7-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="e24d7-109">กฎ ASR บางรายการไม่สนับสนุนข้อยกเว้น</span><span class="sxs-lookup"><span data-stu-id="e24d7-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="e24d7-110">เมื่อต้องการตรวจสอบว่ากฎของคุณสนับสนุนข้อยกเว้นหรือไม่ ให้ดูตาราง กฎ [การลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)การโจมตี</span><span class="sxs-lookup"><span data-stu-id="e24d7-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="e24d7-111">กฎการลดพื้นหน้าของการโจมตี</span><span class="sxs-lookup"><span data-stu-id="e24d7-111">Attack surface reduction rules</span></span>

<span data-ttu-id="e24d7-112">พื้นหน้าการโจมตีขององค์กรของคุณรวมสถานที่ที่ผู้โจมตีอาจโจมตีอุปกรณ์หรือเครือข่ายขององค์กรได้</span><span class="sxs-lookup"><span data-stu-id="e24d7-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="e24d7-113">การลดพื้นหน้าของการโจมตีของคุณหมายถึงการปกป้องอุปกรณ์ขององค์กรและเครือข่าย ซึ่งทิ้งให้ผู้โจมตีมีวิธีการโจมตีลดลง</span><span class="sxs-lookup"><span data-stu-id="e24d7-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="e24d7-114">การกําหนดค่ากฎการลดพื้นหน้าของการโจมตีใน Microsoft Defender for Endpoint สามารถช่วยได้</span><span class="sxs-lookup"><span data-stu-id="e24d7-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="e24d7-115">สำหรับข้อมูลเพิ่มเติม ให้ดู:</span><span class="sxs-lookup"><span data-stu-id="e24d7-115">For more information, see:</span></span>

- [<span data-ttu-id="e24d7-116">แมป GUID ของกฎ ASR กับชื่อ</span><span class="sxs-lookup"><span data-stu-id="e24d7-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="e24d7-117">ความต้องการของกฎ ASR:</span><span class="sxs-lookup"><span data-stu-id="e24d7-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="e24d7-118">Windows 10 Pro เวอร์ชัน 1709 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e24d7-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="e24d7-119">Windows 10 Enterprise เวอร์ชัน 1709 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e24d7-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="e24d7-120">Windows เซิร์ฟเวอร์ เวอร์ชัน 1803 (แชนเนลรายครึ่งปี) หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e24d7-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="e24d7-121">ระบุการยกเว้นที่ถูกต้องที่จะปรับใช้</span><span class="sxs-lookup"><span data-stu-id="e24d7-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="e24d7-122">ค้นหา eventID 1121 หรือ 1122 ใน Microsoft-Windows-Windows Defender/บันทึกการปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="e24d7-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="e24d7-123">ประเมินสถานการณ์การบล็อกและบริบท และยืนยันว่าสถานการณ์นี้ต้องไม่ถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="e24d7-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="e24d7-124">อ่านค่า เส้นทาง ในรายละเอียดเหตุการณ์ ซึ่งเป็นค่าที่กําหนดการยกเว้น</span><span class="sxs-lookup"><span data-stu-id="e24d7-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="e24d7-125">ให้ข้อยกเว้นเคร่งครัดที่สุดเท่าที่จะเป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="e24d7-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="e24d7-126">ใช้อักขระตัวแทนที่ต้องการ (ตัวอย่างเช่น แทนที่ตัวแปรผู้ใช้)</span><span class="sxs-lookup"><span data-stu-id="e24d7-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="e24d7-127">ปรับใช้ข้อยกเว้นตามความต้องการในการปรับใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e24d7-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="e24d7-128">โปรดดูรายละเอียดที่ ปรับแต่ง [กฎการลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)การโจมตี</span><span class="sxs-lookup"><span data-stu-id="e24d7-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="e24d7-129">ไม่รับการยกเว้น</span><span class="sxs-lookup"><span data-stu-id="e24d7-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="e24d7-130">ระบุว่ากฎสนับสนุนข้อยกเว้นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e24d7-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="e24d7-131">ดูรายละเอียดที่ [กฎการลดพื้นหน้าของ](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)การโจมตี</span><span class="sxs-lookup"><span data-stu-id="e24d7-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="e24d7-132">ตรวจทานข้อยกเว้นที่ปรับใช้และตรวจสอบด้วยข้อมูลเหตุการณ์ของอักขระตัวแทนที่พิมพ์ผิดหรือมีแปลผิด</span><span class="sxs-lookup"><span data-stu-id="e24d7-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="e24d7-133">หากต้องการข้อมูลเพิ่มเติม โปรดดูประเภท [การยกเว้นที่ได้รับการสนับสนุน](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="e24d7-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="e24d7-134">ถ้าผลกระทบของกฎสูงเกินไป ให้พิจารณาย้ายกฎ (ย้อนกลับ) ไปยังโหมดตรวจสอบเพื่อการตรวจสอบความถูกต้องเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="e24d7-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="e24d7-135">ดูรายละเอียดที่ [ทดสอบวิธีที่คุณลักษณะของ Microsoft Defender for Endpoint สามารถใช้งานในโหมด](/microsoft-365/security/defender-endpoint/audit-windows-defender)ตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="e24d7-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="e24d7-136">รวบรวมข้อมูลการสนับสนุนเพื่อเปิดกรณีสนับสนุนโดยใช้การสั่งนี้:</span><span class="sxs-lookup"><span data-stu-id="e24d7-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="e24d7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="e24d7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="e24d7-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="e24d7-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
