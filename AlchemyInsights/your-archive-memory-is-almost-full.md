---
title: กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974666"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="87238-102">กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="87238-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="87238-103">ถ้าผู้ใช้ได้รับคำเตือน **กล่องจดหมายเก็บถาวรของคุณเกือบทั้งหมด** หรือคุณจำเป็นต้องเพิ่มขนาดของกล่องจดหมายเก็บถาวรต่อไปนี้คือเคล็ดลับบางประการ:</span><span class="sxs-lookup"><span data-stu-id="87238-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="87238-104">ถ้าผู้ใช้ได้รับมอบหมายให้มี Exchange Online Plan 1 ให้อัปเกรดเป็นสิทธิ์การใช้งาน **Exchange Online plan 2** เพื่อเพิ่มขนาดจาก๕๐กิกะไบต์ถึง100gb</span><span class="sxs-lookup"><span data-stu-id="87238-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="87238-105">ถ้าผู้ใช้ได้รับมอบหมายอย่างใดอย่างหนึ่งต่อไปนี้: **Exchange Online plan 2** หรือ Exchange online plan 1 ที่มี Add-on ของ exchange Online ที่เก็บถาวรให้ใช้ขั้นตอนด้านล่างนี้เพื่อเปิดใช้งานการเก็บถาวรแบบขยายโดยอัตโนมัติ:</span><span class="sxs-lookup"><span data-stu-id="87238-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="87238-106">[เชื่อมต่อกับ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="87238-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="87238-107">เรียกใช้ commandlet ต่อไปนี้สำหรับผู้ใช้:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="87238-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="87238-108">เรียกใช้ commandlet ต่อไปนี้เพื่อยืนยันว่ามีการเปิดใช้งานสำหรับผู้ใช้:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="87238-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="87238-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="87238-109">For more information see:</span></span>

- [<span data-ttu-id="87238-110"> เปิดใช้งานการเก็บถาวรแบบไม่จำกัด-วิธีใช้สำหรับผู้ดูแลระบบ-Microsoft ๓๖๕การปฏิบัติตามข้อบังคับ | Microsoft เอกสาร</span><span class="sxs-lookup"><span data-stu-id="87238-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="87238-111">ข้อจำกัดของ Exchange Online-คำอธิบายบริการ | Microsoft เอกสาร</span><span class="sxs-lookup"><span data-stu-id="87238-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="87238-112">อัปเกรดเป็นแผนธุรกิจที่แตกต่างกัน Microsoft เอกสาร</span><span class="sxs-lookup"><span data-stu-id="87238-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

