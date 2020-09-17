---
title: ปัญหาเกี่ยวกับการหลอกลวงฟิชชิ่งหรือการเลียนแบบใช่หรือไม่
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: 92e7f611b08a5457e52be248982785b2dc2ddabc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773038"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="4c587-102">ปัญหาเกี่ยวกับการหลอกลวงฟิชชิ่งหรือการเลียนแบบใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="4c587-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="4c587-103">เรียนรู้วิธีที่ Microsoft ปกป้องคุณจาก:</span><span class="sxs-lookup"><span data-stu-id="4c587-103">Learn how Microsoft protects you from:</span></span>

- [<span data-ttu-id="4c587-104">ปลอมแปลง</span><span class="sxs-lookup"><span data-stu-id="4c587-104">Spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)

- [<span data-ttu-id="4c587-105">ฟิชชิ่งและการเลียนแบบ</span><span class="sxs-lookup"><span data-stu-id="4c587-105">Phishing and impersonation</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)

<span data-ttu-id="4c587-106">คำแนะนำเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="4c587-106">Additional recommendations:</span></span>

- <span data-ttu-id="4c587-107">สำหรับผู้ส่งปลอมที่ปรากฏมาจากโดเมนของคุณเอง [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) และ [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) สามารถช่วยคุณได้</span><span class="sxs-lookup"><span data-stu-id="4c587-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="4c587-108">ตรวจสอบผู้ส่งในโดเมนของคุณเองไม่ได้รับการกำหนดค่าให้ข้ามการกรองป้องกันสแปมโดยใช้กฎโฟลว์จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน) หรืออนุญาตรายการ</span><span class="sxs-lookup"><span data-stu-id="4c587-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="4c587-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่ข้อควรระวังเกี่ยวกับการข้าม[ตัวกรองสแปมของ Microsoft](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)</span><span class="sxs-lookup"><span data-stu-id="4c587-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="4c587-110">ตรวจสอบว่าผู้ใช้ไม่ได้กำหนดค่ารายการ [รายชื่อผู้ส่งที่ปลอดภัย](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) ที่อาจทำให้การโจมตีของฟิชชิ่ง</span><span class="sxs-lookup"><span data-stu-id="4c587-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="4c587-111">พิจารณาส่งข้อความอีเมลที่เชื่อถือได้และฟิชชิ่งเป็นการกักกันแทนที่จะเป็นโฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="4c587-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="4c587-112">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ข้อความอีเมลที่ถูกกักกัน](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)</span><span class="sxs-lookup"><span data-stu-id="4c587-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages).</span></span>

<span data-ttu-id="4c587-113">**การ[รายงานข้อความไปยัง Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)เป็นวิธีที่ดีที่สุดในการแจ้งให้เราทราบว่าตัวกรองกำลังดำเนินการอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="4c587-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
