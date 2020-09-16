---
title: การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727802"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="a441f-102">การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="a441f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="a441f-103">ผลลัพธ์ของฟังก์ชัน eDiscovery ใหม่และได้รับการปรับปรุงในศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕จะมีการถอนเครื่องมือ eDiscovery และ commandlet ดังต่อไปนี้ในเดือนที่จะมาถึงดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a441f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="a441f-104">[EDiscovery ในสถาน](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ที่และ [ในสถานที่ถือ](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="a441f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="a441f-105">Cmdlet PowerShell ของ Exchange Online ที่สนับสนุน eDiscovery ในสถานที่และในตำแหน่งที่ถือ</span><span class="sxs-lookup"><span data-stu-id="a441f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="a441f-106">(Cmdlet เหล่านี้จะมีการระบุเป็น \*-MailboxSearch cmdlets) ซึ่งรวมถึง cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a441f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="a441f-107">MailboxSearch ใหม่</span><span class="sxs-lookup"><span data-stu-id="a441f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="a441f-108">เริ่มต้น-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a441f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="a441f-109">หยุด-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a441f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="a441f-110">ตั้งค่า-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a441f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="a441f-111">Cmdlet [กล่องจดหมายการค้นหา](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ใน Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a441f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="a441f-112">การดำเนินการต่อไปนี้ใน API เว็บเซอร์วิสของ Exchange:</span><span class="sxs-lookup"><span data-stu-id="a441f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="a441f-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a441f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="a441f-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a441f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="a441f-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a441f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="a441f-116">ขั้นสูง eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="a441f-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="a441f-117">**ไทม์ไลน์สำหรับการเกษียณอายุ**:</span><span class="sxs-lookup"><span data-stu-id="a441f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="a441f-118">**1 กรกฎาคม๒๐๒๐** คุณไม่สามารถสร้างการค้นหาใหม่และจัดเก็บได้อีกต่อไปแต่คุณสามารถเรียกใช้แก้ไขและลบการค้นหาที่มีอยู่ได้ด้วยความเสี่ยงของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="a441f-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="a441f-119">ฝ่ายสนับสนุนของ Microsoft ไม่สนับสนุนการใช้ eDiscovery ในตำแหน่งที่ & อยู่ใน EAC อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="a441f-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="a441f-120">**1 ตุลาคม๒๐๒๐** & eDiscovery ในสถานที่มีฟังก์ชันการทำงานใน EAC จะถูกวางไว้ในโหมดอ่านอย่างเดียวเพื่อให้คุณสามารถเอาการค้นหาที่มีอยู่และการค้นหาที่มีอยู่ออกได้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="a441f-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="a441f-121">**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:</span><span class="sxs-lookup"><span data-stu-id="a441f-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="a441f-122">โยกย้ายการค้นหา eDiscovery ดั้งเดิมและถือเป็นศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="a441f-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="a441f-123">การเกษียณอายุของเครื่องมือ eDiscovery ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="a441f-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="a441f-124">คำถามที่ถามบ่อยเกี่ยวกับ eDiscovery ในสถานที่และในสถานที่ถือ</span><span class="sxs-lookup"><span data-stu-id="a441f-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



