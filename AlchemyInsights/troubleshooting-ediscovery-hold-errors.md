---
title: การแก้ไขปัญหา ediscovery มีข้อผิดพลาด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676285"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="3fc9a-102">การแก้ไขปัญหา ediscovery มีข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="3fc9a-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="3fc9a-103">พบปัญหาเกี่ยวกับการหยุด eDiscovery ใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="3fc9a-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="3fc9a-104">ต่อไปนี้เป็นหลักปฏิบัติที่ดีที่สุดบางอย่างที่ควรพิจารณา:</span><span class="sxs-lookup"><span data-stu-id="3fc9a-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="3fc9a-105">ตรวจสอบสถานะการกระจายการหยุด</span><span class="sxs-lookup"><span data-stu-id="3fc9a-105">Check the hold distribution status.</span></span>  <span data-ttu-id="3fc9a-106">ถ้า สถานะ เป็น **เปิด (รอการรอการ)** **หรือ ปิด (รอ** การค้างอยู่) รอให้การแจกแจงหยุดเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="3fc9a-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="3fc9a-107">ผสาน eDiscovery จะหยุดการอัปเดตเป็นคําขอแบบกลุ่มเดียวแทนการอัปเดตนโยบายซ้ําๆ ในแต่ละทรานแซคชัน</span><span class="sxs-lookup"><span data-stu-id="3fc9a-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="3fc9a-108">เรียกใช้ Set-CaseHoldPolicy <policyname> -RetryDistribution ใน Powershell ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="3fc9a-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="3fc9a-109">For details, see[เชื่อมต่อ to security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3fc9a-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="3fc9a-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="3fc9a-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="3fc9a-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="3fc9a-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
