---
title: การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650587"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="159f3-102">การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="159f3-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="159f3-103">จากฟังก์ชัน eDiscovery ใหม่ ที่ได้รับการปรับปรุงในศูนย์การปฏิบัติตามกฎระเบียบ 365 Microsoft เครื่องมือ eDiscovery แบบดั้งเดิมและ commandlets ต่อไปนี้จะออกใช้ในเดือนที่จะมาถึง:</span><span class="sxs-lookup"><span data-stu-id="159f3-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="159f3-104">การหยุดพักในสถานที่[eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)และ[ในสถานที่](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)ในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="159f3-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="159f3-105">Cmdlet แบบออนไลน์ของอัตราแลกเปลี่ยนที่สนับสนุน eDiscovery ในสถานที่และในสถานที่</span><span class="sxs-lookup"><span data-stu-id="159f3-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="159f3-106">(cmdlet เหล่านี้ถูกระบุรวมเป็น cmdlet กล่องจดหมาย Search) ซึ่งรวมถึง cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="159f3-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="159f3-107">กล่องจดหมายใหม่ค้นหา</span><span class="sxs-lookup"><span data-stu-id="159f3-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="159f3-108">กล่องจดหมายเริ่มต้นค้นหา</span><span class="sxs-lookup"><span data-stu-id="159f3-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="159f3-109">หยุดการค้นหากล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="159f3-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="159f3-110">ตั้งค่ากล่องจดหมายค้นหา</span><span class="sxs-lookup"><span data-stu-id="159f3-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="159f3-111">คําสั่งจัดการ[กล่องจดหมายการค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="159f3-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="159f3-112">การดําเนินการต่อไปนี้ใน API บริการเว็บอัตราแลกเปลี่ยน:</span><span class="sxs-lookup"><span data-stu-id="159f3-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="159f3-113">รับกล่องจดหมายที่ค้นหาได้</span><span class="sxs-lookup"><span data-stu-id="159f3-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="159f3-114">ตั้งค่าการระงับบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="159f3-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="159f3-115">การฝากข้อความ</span><span class="sxs-lookup"><span data-stu-id="159f3-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="159f3-116">ขั้นสูง eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="159f3-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="159f3-117">**ระยะเวลาเกษียณ :**</span><span class="sxs-lookup"><span data-stu-id="159f3-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="159f3-118">1 เมษายน 2020: คุณจะไม่สามารถสร้างการค้นหาและการระงับใหม่ได้ แต่คุณยังสามารถเรียกใช้ แก้ไข และลบการค้นหาที่มีอยู่ตามความเสี่ยงของคุณเองได้</span><span class="sxs-lookup"><span data-stu-id="159f3-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="159f3-119">ฝ่ายสนับสนุนของ Microsoft จะไม่สนับสนุน & eDiscovery ในตําแหน่งใน EAC อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="159f3-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="159f3-120">1 กรกฎาคม 2020: & eDiscovery ในสถานที่เก็บใน EAC จะถูกวางในโหมดอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="159f3-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="159f3-121">ซึ่งหมายความว่าคุณจะสามารถลบการค้นหาที่มีอยู่และระงับได้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="159f3-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="159f3-122">**สําหรับข้อมูลเพิ่มเติม โปรดดูที่**:</span><span class="sxs-lookup"><span data-stu-id="159f3-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="159f3-123">โยกย้ายการค้นหา eDiscovery ดั้งเดิมและระงับไปยังศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="159f3-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="159f3-124">การเกษียณอายุของเครื่องมือ eDiscovery แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="159f3-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="159f3-125">คําถามที่พบบ่อยเกี่ยวกับ อิน-เพลส</span><span class="sxs-lookup"><span data-stu-id="159f3-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



