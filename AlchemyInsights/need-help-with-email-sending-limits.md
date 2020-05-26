---
title: ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลใช่ไหม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358360"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="17ed1-102">ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="17ed1-102">Need help with email sending limits?</span></span>

<span data-ttu-id="17ed1-103">ด้านล่างเป็น**โดยการออกแบบขีดจํากัดการส่ง**บังคับในการให้บริการ</span><span class="sxs-lookup"><span data-stu-id="17ed1-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="17ed1-104">ข้อมูลเพิ่มเติมเกี่ยวกับข้อจํากัดเหล่านี้ได้รับการบันทึกไว้[ที่นี่](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="17ed1-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="17ed1-105">เพื่อกีดกันการส่งข้อความจํานวนมากที่ไม่พึงประสงค์เราใช้**วงเงินอัตราผู้รับต่อผู้ใช้ไปยังข้อความขาออกและข้อความภายในทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="17ed1-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="17ed1-106">ใน SKU ทั้งหมด ขีดจํากัดนี้ผู้รับ**10,000 ต่อวัน**</span><span class="sxs-lookup"><span data-stu-id="17ed1-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="17ed1-107">ลูกค้าที่ต้องการส่งอีเมลเชิงพาณิชย์จํานวนมากที่ถูกต้องตามกฎหมาย (เช่น จดหมายข่าวของลูกค้า) ควรใช้ผู้ให้บริการบุคคลที่สามที่มีความเชี่ยวชาญในบริการเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="17ed1-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="17ed1-108">**หมายเหตุ**: เมื่อถึงขีดจํากัดอัตราผู้รับข้อความไม่สามารถส่งข้อความจากกล่องจดหมายจนกว่าจํานวนผู้รับข้อความที่ส่งข้อความในช่วง 24 ชั่วโมงที่ผ่านมาลดลงต่ํากว่าขีด จํากัด</span><span class="sxs-lookup"><span data-stu-id="17ed1-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="17ed1-109">ผู้ใช้จะไม่สามารถส่งข้อความได้จนกว่าจะถึงจุดนั้น</span><span class="sxs-lookup"><span data-stu-id="17ed1-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="17ed1-110">มีการใช้ขีดจํากัดอัตราข้อความ**30 ข้อความต่อนาที**ใน SKU ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="17ed1-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="17ed1-111">ซึ่งกําหนดจํานวนข้อความที่ผู้ใช้สามารถส่งจากบัญชีผู้ใช้ Exchange แบบออนไลน์ภายในรอบระยะเวลาที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="17ed1-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="17ed1-112">**จํานวนสูงสุดของผู้รับที่อนุญาตในฟิลด์ ถึง สําเนาถึง และสําเนาลับถึง**สําหรับข้อความอีเมลเดียว**1000 recipients**</span><span class="sxs-lookup"><span data-stu-id="17ed1-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="17ed1-113">เมื่อต้องการกําหนดขีดจํากัดนี้เอง ให้ไปที่[ที่นี่](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="17ed1-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
