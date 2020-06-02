---
title: ปัญหาเกี่ยวกับการปลอมแปลง ฟิชชิ่ง หรือการปลอมตัว
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: fb10c486833cfb0a1726dce69bc2176b39565e9d
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510051"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="6ca36-102">ปัญหาเกี่ยวกับการปลอมแปลง ฟิชชิ่ง หรือการปลอมตัว</span><span class="sxs-lookup"><span data-stu-id="6ca36-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="6ca36-103">เรียนรู้วิธีที่ Microsoft ปกป้องคุณจาก:</span><span class="sxs-lookup"><span data-stu-id="6ca36-103">Learn how Microsoft protects you from:</span></span>

- [<span data-ttu-id="6ca36-104">การปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="6ca36-104">Spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)

- [<span data-ttu-id="6ca36-105">ฟิชชิงและการปลอมตัว</span><span class="sxs-lookup"><span data-stu-id="6ca36-105">Phishing and impersonation</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)

<span data-ttu-id="6ca36-106">คําแนะนําเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="6ca36-106">Additional recommendations:</span></span>

- <span data-ttu-id="6ca36-107">สําหรับผู้ส่งปลอมที่ดูเหมือนจะมาจากโดเมนของคุณเอง[SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)และ[DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)สามารถช่วยได้</span><span class="sxs-lookup"><span data-stu-id="6ca36-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="6ca36-108">ตรวจสอบว่าผู้ส่งในโดเมนของคุณไม่ได้ถูกกําหนดค่าให้ข้ามการกรองสแปมโดยใช้กฎการไหลของจดหมาย (หรือที่เรียกว่ากฎการขนส่ง) หรืออนุญาตรายการ</span><span class="sxs-lookup"><span data-stu-id="6ca36-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="6ca36-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ข้อควรระวังในการข้ามตัวกรองสแปมของ Microsoft](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)</span><span class="sxs-lookup"><span data-stu-id="6ca36-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="6ca36-110">ตรวจสอบว่าผู้ใช้ไม่ได้กําหนดค่ารายการ[รายชื่อผู้ส่งที่ปลอดภัย](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)ซึ่งอาจอนุญาตให้มีการโจมตีแบบฟิชชิ่งได้</span><span class="sxs-lookup"><span data-stu-id="6ca36-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="6ca36-111">ลองส่งสแปมและข้อความฟิชชิงที่มีความเชื่อมั่นสูงเพื่อกักกันแทนที่จะใช้โฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="6ca36-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="6ca36-112">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[กักกันข้อความอีเมล](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)</span><span class="sxs-lookup"><span data-stu-id="6ca36-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages).</span></span>

<span data-ttu-id="6ca36-113">**[การรายงานข้อความไปยัง Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)คือวิธีที่ดีที่สุดในการแจ้งให้เราทราบว่าตัวกรองมีประสิทธิภาพเพียงใด**</span><span class="sxs-lookup"><span data-stu-id="6ca36-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
