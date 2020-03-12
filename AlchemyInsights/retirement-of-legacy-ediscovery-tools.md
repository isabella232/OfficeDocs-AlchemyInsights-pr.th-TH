---
title: การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600403"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="81d96-102">การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="81d96-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="81d96-103">เป็นผลมาจากฟังก์ชัน eDiscovery ใหม่และปรับปรุงแล้วใน Microsoft ๓๖๕ศูนย์ปฏิบัติตามกฎระเบียบเครื่องมือ eDiscovery แบบดั้งเดิมต่อไปนี้และ commandlets จะถูกยกเลิกในเดือนที่จะมาถึง:</span><span class="sxs-lookup"><span data-stu-id="81d96-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="81d96-104">[ในตำแหน่ง eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)และ[ในตำแหน่ง](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)ที่เก็บอยู่ในศูนย์ดูแลอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="81d96-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="81d96-105">Cmdlets PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนที่สนับสนุน eDiscovery ในตำแหน่งและในสถานที่เก็บ</span><span class="sxs-lookup"><span data-stu-id="81d96-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="81d96-106">(Cmdlets เหล่านี้จะมีการระบุรวมเป็น \*-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ของต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="81d96-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="81d96-107">MailboxSearch ใหม่</span><span class="sxs-lookup"><span data-stu-id="81d96-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="81d96-108">เริ่มต้น-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81d96-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="81d96-109">หยุด-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81d96-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="81d96-110">ชุด-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81d96-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="81d96-111">Cmdlet[กล่องจดหมายค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="81d96-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="81d96-112">การดำเนินการต่อไปนี้ใน API บริการเว็บของอัตราแลกเปลี่ยน:</span><span class="sxs-lookup"><span data-stu-id="81d96-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="81d96-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="81d96-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="81d96-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="81d96-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="81d96-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="81d96-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="81d96-116">โปรแกรม Office ๓๖๕ขั้นสูง eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="81d96-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="81d96-117">**ระยะเวลาสำหรับการเกษียณอายุ**:</span><span class="sxs-lookup"><span data-stu-id="81d96-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="81d96-118">วันที่1เมษายน๒๐๒๐: คุณจะไม่สามารถสร้างการค้นหาใหม่และเก็บไว้ได้แต่คุณยังสามารถเรียกใช้แก้ไขและลบการค้นหาที่มีอยู่ได้ด้วยความเสี่ยงของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="81d96-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="81d96-119">ฝ่ายสนับสนุนของ Microsoft จะไม่สนับสนุนในตำแหน่ง eDiscovery & ในแบบ EAC</span><span class="sxs-lookup"><span data-stu-id="81d96-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="81d96-120">1กรกฎาคม๒๐๒๐: & eDiscovery ในสถานที่เก็บฟังก์ชันในแบบ EAC จะถูกวางในโหมดอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="81d96-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="81d96-121">ซึ่งหมายความว่าคุณจะสามารถลบการค้นหาที่มีอยู่และถือได้</span><span class="sxs-lookup"><span data-stu-id="81d96-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="81d96-122">**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:</span><span class="sxs-lookup"><span data-stu-id="81d96-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="81d96-123">ย้ายการค้นหา eDiscovery ดั้งเดิมและถือเป็นศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="81d96-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="81d96-124">การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="81d96-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="81d96-125">คำถามที่พบบ่อยเกี่ยวกับ eDiscovery ในสถานที่และในสถานที่ถือ</span><span class="sxs-lookup"><span data-stu-id="81d96-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



