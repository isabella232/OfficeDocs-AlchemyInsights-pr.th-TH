---
title: ปัญหาเกี่ยวกับการปลอมแปลงฟิชชิ่งหรือการเลียนแบบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: 73a960d76802ccfee5500b1816f34a15b960c3f2
ms.sourcegitcommit: 7398c9d81f00328d1edc515a195d779dd28f1bea
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/03/2019
ms.locfileid: "36716122"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="9e96e-102">ปัญหาเกี่ยวกับการปลอมแปลงฟิชชิ่งหรือการเลียนแบบ</span><span class="sxs-lookup"><span data-stu-id="9e96e-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="9e96e-103">เรียนรู้วิธีที่ Office ๓๖๕ปกป้องคุณจาก:</span><span class="sxs-lookup"><span data-stu-id="9e96e-103">Learn how Office 365 protects you from:</span></span>

- [<span data-ttu-id="9e96e-104">ปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="9e96e-104">Spoofing</span></span>](https://docs.microsoft.com/office365/securitycompliance/anti-spoofing-protection)

- [<span data-ttu-id="9e96e-105">การฟิชชิ่งและการเลียนแบบ</span><span class="sxs-lookup"><span data-stu-id="9e96e-105">Phishing and impersonation</span></span>](https://docs.microsoft.com/office365/securitycompliance/atp-anti-phishing)

<span data-ttu-id="9e96e-106">คำแนะนำเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="9e96e-106">Additional recommendations:</span></span>

- <span data-ttu-id="9e96e-107">สำหรับผู้ส่งที่ถูกปลอมแปลงที่ปรากฏขึ้นมาจากโดเมนของคุณเอง[SPF](https://docs.microsoft.com/office365/securitycompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)และ[DKIM](https://docs.microsoft.com/office365/securitycompliance/use-dkim-to-validate-outbound-email)สามารถช่วยได้</span><span class="sxs-lookup"><span data-stu-id="9e96e-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/office365/securitycompliance/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/office365/securitycompliance/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="9e96e-108">ตรวจสอบผู้ส่งในโดเมนของคุณเองไม่ได้รับการกำหนดค่าให้ข้ามการกรองป้องกันสแปมโดยใช้กฎของลำดับจดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน) หรืออนุญาตให้รายการรายการ</span><span class="sxs-lookup"><span data-stu-id="9e96e-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="9e96e-109">สำหรับข้อมูลเพิ่มเติมโปรดดูที่ข้อ[ควรระวังกับการข้ามตัวกรองสแปมของ Office ๓๖๕](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)</span><span class="sxs-lookup"><span data-stu-id="9e96e-109">For more information, see [Cautions against bypassing Office 365 spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="9e96e-110">ตรวจสอบว่าผู้ใช้ไม่ได้กำหนดค่ารายการ[รายชื่อผู้ส่งที่ปลอดภัย](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)ที่อาจทำให้เกิดการโจมตีแบบฟิชชิ่งได้</span><span class="sxs-lookup"><span data-stu-id="9e96e-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="9e96e-111">พิจารณาส่งจดหมายขยะและข้อความที่เชื่อถือได้สูงเพื่อกักกันแทนที่จะเป็นโฟลเดอร์เมลขยะ</span><span class="sxs-lookup"><span data-stu-id="9e96e-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="9e96e-112">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[ข้อความใน Office ๓๖๕](https://docs.microsoft.com/office365/securitycompliance/quarantine-email-messages)</span><span class="sxs-lookup"><span data-stu-id="9e96e-112">For more information, see [Quarantine email messages in Office 365](https://docs.microsoft.com/office365/securitycompliance/quarantine-email-messages).</span></span>

<span data-ttu-id="9e96e-113">**[การรายงานข้อความไปยัง Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)เป็นวิธีที่ดีที่สุดในการแจ้งให้เราทราบว่าตัวกรองมีประสิทธิภาพอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="9e96e-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
