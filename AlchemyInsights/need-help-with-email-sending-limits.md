---
title: ต้องการความช่วยเหลือในการจำกัดการส่งอีเมลหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702382"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="d9d47-102">ต้องการความช่วยเหลือในการจำกัดการส่งอีเมลหรือไม่</span><span class="sxs-lookup"><span data-stu-id="d9d47-102">Need help with email sending limits?</span></span>

<span data-ttu-id="d9d47-103">ด้านล่างนี้คือ **ขีดจำกัดการส่งโดยการออกแบบ** ที่บังคับใช้ในบริการ</span><span class="sxs-lookup"><span data-stu-id="d9d47-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="d9d47-104">ข้อมูลเพิ่มเติมเกี่ยวกับขีดจำกัดเหล่านี้จะได้รับการบันทึกไว้[ที่นี่](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="d9d47-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="d9d47-105">เมื่อต้องการกีดกันการนำส่งข้อความจำนวนมากที่ไม่พึงประสงค์เราจะนำข้อ**จำกัดอัตราผู้รับต่อผู้ใช้ไปใช้กับข้อความขาออกและข้อความภายในทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="d9d47-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="d9d47-106">ใน Sku ทั้งหมดขีดจำกัดนี้คือ**ผู้รับ๑๐,๐๐๐ต่อวัน**</span><span class="sxs-lookup"><span data-stu-id="d9d47-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="d9d47-107">ลูกค้าที่จำเป็นต้องส่งอีเมลการค้าจำนวนมากที่ถูกต้องตามกฎหมาย (ตัวอย่างเช่นจดหมายข่าวของลูกค้า) ควรใช้ผู้ให้บริการของบริษัทอื่นที่มีความเชี่ยวชาญในบริการเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="d9d47-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="d9d47-108">**หมายเหตุ**: เมื่อถึงขีดจำกัดอัตราผู้รับข้อความจะไม่สามารถส่งจากกล่องจดหมายได้จนกว่าจำนวนผู้รับที่ส่งข้อความในช่วง24ชั่วโมงที่ผ่านมาจะลดลงต่ำกว่าขีดจำกัด</span><span class="sxs-lookup"><span data-stu-id="d9d47-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="d9d47-109">ผู้ใช้จะไม่สามารถส่งข้อความได้จนกว่าจุดนั้น</span><span class="sxs-lookup"><span data-stu-id="d9d47-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="d9d47-110">ขีดจำกัดอัตราข้อความ **30 ข้อความต่อนาที** จะถูกนำไปใช้ใน sku ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="d9d47-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="d9d47-111">สิ่งนี้จะกำหนดจำนวนข้อความที่ผู้ใช้สามารถส่งจากบัญชีผู้ใช้ Exchange Online ของพวกเขาภายในช่วงเวลาที่ระบุได้</span><span class="sxs-lookup"><span data-stu-id="d9d47-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="d9d47-112">**จำนวนสูงสุดของผู้รับที่ได้รับอนุญาตในเขตข้อมูลถึง, สำเนาถึงและสำเนาลับ**ถึงสำหรับข้อความอีเมลเดียวทั้งหมดจะเป็น**ผู้รับ๑๐๐๐**</span><span class="sxs-lookup"><span data-stu-id="d9d47-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="d9d47-113">เมื่อต้องการกำหนดขีดจำกัดนี้เองให้ไป[ที่นี่](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="d9d47-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
