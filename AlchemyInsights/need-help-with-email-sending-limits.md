---
title: ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลหรือไม่
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836298"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="7ebba-102">ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลหรือไม่</span><span class="sxs-lookup"><span data-stu-id="7ebba-102">Need help with email sending limits?</span></span>

<span data-ttu-id="7ebba-103">ด้านล่างนี้คือ **ขีดจํากัดการส่งตาม** การออกแบบที่ถูกบังคับใช้ในบริการ</span><span class="sxs-lookup"><span data-stu-id="7ebba-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="7ebba-104">ข้อมูลเพิ่มเติมเกี่ยวกับขีดจํากัดเหล่านี้ได้บันทึก[ที่นี่](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="7ebba-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="7ebba-105">ในการลบการส่งข้อความเป็นกลุ่มที่ไม่พึงประสงค์ เราจะใช้ขีดจํากัดอัตราของผู้รับต่อ **ผู้ใช้กับข้อความขาออกและข้อความ** ภายในทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7ebba-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="7ebba-106">ใน SKU ทั้งหมด ขีดจํากัดคือ **10,000 คน** ต่อวัน</span><span class="sxs-lookup"><span data-stu-id="7ebba-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="7ebba-107">ลูกค้าที่ต้องการส่งอีเมลเชิงพาณิชย์เป็นกลุ่มที่ถูกต้องตามกฎหมาย (ตัวอย่างเช่น จดหมายข่าวลูกค้า) ควรใช้ผู้ให้บริการของบริษัทอื่นที่ขายดีในบริการเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="7ebba-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="7ebba-108">**หมายเหตุ**: เมื่อถึงขีดจํากัดอัตราของผู้รับข้อความแล้ว ไม่สามารถส่งข้อความจากกล่องจดหมายได้จนกว่าจะถึงจํานวนผู้รับที่ส่งข้อความในช่วง 24 ชั่วโมงที่ผ่านมาลดขีดจํากัด</span><span class="sxs-lookup"><span data-stu-id="7ebba-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="7ebba-109">ผู้ใช้จะไม่สามารถส่งข้อความได้จนกว่าจะถึงจุดนั้น</span><span class="sxs-lookup"><span data-stu-id="7ebba-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="7ebba-110">ขีดจํากัดอัตราข้อความ **30 ข้อความต่อ** นาทีจะถูกปรับใช้ใน SKU ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7ebba-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="7ebba-111">ซึ่งระบุปริมาณข้อความที่ผู้ใช้สามารถส่งจากบัญชี Exchange Online ภายในช่วงเวลาที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="7ebba-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="7ebba-112">จํานวน **ผู้รับสูงสุดที่อนุญาตใน** เขตข้อมูล ถึงส.ค. และ ส. ของข้อความอีเมลเดียว ใน SKU ทั้งหมด คือ **1000** ผู้รับ</span><span class="sxs-lookup"><span data-stu-id="7ebba-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="7ebba-113">เมื่อต้องการปรับแต่งขีดจํากัดนี้ [ให้ไปที่](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)นี่</span><span class="sxs-lookup"><span data-stu-id="7ebba-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
