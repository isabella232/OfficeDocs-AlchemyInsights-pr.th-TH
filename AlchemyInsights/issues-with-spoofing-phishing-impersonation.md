---
title: ปัญหาเกี่ยวกับการปลอมแปลงฟิชชิ่งหรือการเลียนแบบ?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: fa6503b7ec1c4e83030149ee460e6d84602d7f4d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713989"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="0f20a-102">ปัญหาเกี่ยวกับการปลอมแปลงฟิชชิ่งหรือการเลียนแบบ?</span><span class="sxs-lookup"><span data-stu-id="0f20a-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="0f20a-103">เรียนรู้วิธีที่ Microsoft ปกป้องคุณจาก:</span><span class="sxs-lookup"><span data-stu-id="0f20a-103">Learn how Microsoft protects you from:</span></span>

- [<span data-ttu-id="0f20a-104">การปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="0f20a-104">Spoofing</span></span>](https://docs.microsoft.com/office365/securitycompliance/anti-spoofing-protection)

- [<span data-ttu-id="0f20a-105">ฟิชชิ่งและการเลียนแบบ</span><span class="sxs-lookup"><span data-stu-id="0f20a-105">Phishing and impersonation</span></span>](https://docs.microsoft.com/office365/securitycompliance/atp-anti-phishing)

<span data-ttu-id="0f20a-106">คําแนะนําเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="0f20a-106">Additional recommendations:</span></span>

- <span data-ttu-id="0f20a-107">สําหรับผู้ส่งปลอมที่ดูเหมือนว่ามาจากโดเมนของคุณเอง[SPF](https://docs.microsoft.com/office365/securitycompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)และ[DKIM](https://docs.microsoft.com/office365/securitycompliance/use-dkim-to-validate-outbound-email)สามารถช่วยคุณได้</span><span class="sxs-lookup"><span data-stu-id="0f20a-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/office365/securitycompliance/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/office365/securitycompliance/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="0f20a-108">ตรวจสอบผู้ส่งในโดเมนของคุณเองไม่ได้ถูกกําหนดค่าให้ข้ามการกรองสแปมโดยใช้กฎขั้นตอนจดหมาย (หรือที่เรียกอีกอย่างว่ากฎการขนส่ง) หรืออนุญาตรายการรายการ</span><span class="sxs-lookup"><span data-stu-id="0f20a-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="0f20a-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ข้อควรระวังในการข้ามตัวกรองสแปมของ Microsoft](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)</span><span class="sxs-lookup"><span data-stu-id="0f20a-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="0f20a-110">ตรวจสอบว่าผู้ใช้ไม่ได้กําหนดค่ารายการ[ผู้ส่งที่ปลอดภัย](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)ที่อาจทําให้การโจมตีแบบฟิชชิ่ง</span><span class="sxs-lookup"><span data-stu-id="0f20a-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="0f20a-111">พิจารณาการส่งข้อความสแปมและฟิชชิ่งที่มีความเชื่อมั่นสูงเพื่อกักกันแทนโฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="0f20a-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="0f20a-112">สําหรับข้อมูลเพิ่มเติม โปรดดูที่[กักเก็บข้อความอีเมล](https://docs.microsoft.com/office365/securitycompliance/quarantine-email-messages)</span><span class="sxs-lookup"><span data-stu-id="0f20a-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/office365/securitycompliance/quarantine-email-messages).</span></span>

<span data-ttu-id="0f20a-113">**[การรายงานข้อความไปยัง Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)เป็นวิธีที่ดีที่สุดในการแจ้งให้เราทราบว่าตัวกรองมีประสิทธิภาพเป็นอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="0f20a-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
