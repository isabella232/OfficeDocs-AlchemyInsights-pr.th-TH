---
title: เครื่องมือ eDiscovery ดั้งเดิมเกษียณ
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798568"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="fd6ab-102">เครื่องมือ eDiscovery ดั้งเดิมเกษียณ</span><span class="sxs-lookup"><span data-stu-id="fd6ab-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="fd6ab-103">เนื่องจากฟังก์ชัน eDiscovery ใหม่และที่ปรับปรุงแล้วในศูนย์การปฏิบัติตามข้อบังคับของ Microsoft 365 เครื่องมือ eDiscovery ดั้งเดิมและ commandlets ต่อไปนี้จะถูกปลดระวางในเดือนต่อๆ ไป:</span><span class="sxs-lookup"><span data-stu-id="fd6ab-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="fd6ab-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [และ In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in-Place ใน Exchange admin center</span><span class="sxs-lookup"><span data-stu-id="fd6ab-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="fd6ab-105">cmdlet PowerShell ของ Exchange Online ที่สนับสนุนIn-Place eDiscovery In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="fd6ab-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="fd6ab-106">(cmdlet เหล่านี้จะถูกระบุโดยรวมว่า \*-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fd6ab-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="fd6ab-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fd6ab-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="fd6ab-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fd6ab-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="fd6ab-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fd6ab-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="fd6ab-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fd6ab-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="fd6ab-111">cmdlet [ของ](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) กล่องจดหมายการค้นหาใน Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fd6ab-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="fd6ab-112">การดําเนินการต่อไปนี้ใน API ของ Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="fd6ab-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="fd6ab-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd6ab-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="fd6ab-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd6ab-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="fd6ab-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd6ab-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="fd6ab-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="fd6ab-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="fd6ab-117">**ไทม์ไลน์ปลดการเกษียณ**:</span><span class="sxs-lookup"><span data-stu-id="fd6ab-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="fd6ab-118">**1 กรกฎาคม 2020** คุณไม่สามารถสร้างการค้นหาและการหยุดใหม่ได้อีกต่อไป แต่คุณสามารถเรียกใช้ แก้ไข และลบการค้นหาที่มีอยู่โดยคุณต้องยอมรับความเสี่ยงของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="fd6ab-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="fd6ab-119">การสนับสนุนของ Microsoft ไม่สนับสนุนIn-Place eDiscovery & Holds ใน EAC อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="fd6ab-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="fd6ab-120">**1 ตุลาคม 2020** In-Place & eDiscovery & Holds ใน EAC จะถูกวางในโหมดอ่านอย่างเดียว เพื่อให้คุณสามารถลบการค้นหาและการหยุดที่มีอยู่เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="fd6ab-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="fd6ab-121">**หากต้องการข้อมูลเพิ่มเติม โปรดดู**:</span><span class="sxs-lookup"><span data-stu-id="fd6ab-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="fd6ab-122">โยกย้ายการค้นหา eDiscovery ดั้งเดิมและหยุดไปยังศูนย์การปฏิบัติตามข้อบังคับของ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fd6ab-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="fd6ab-123">การเกษียณเครื่องมือ eDiscovery ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="fd6ab-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="fd6ab-124">Faq about In-Place eDiscovery and In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="fd6ab-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



