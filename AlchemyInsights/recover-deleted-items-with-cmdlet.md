---
title: กู้คืนรายการที่ถูกลบด้วย cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493427"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="8ddb5-102">กู้คืนรายการที่ถูกลบด้วย cmdlet</span><span class="sxs-lookup"><span data-stu-id="8ddb5-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="8ddb5-103">ใช้ cmdlet[รับการกู้คืนItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)เพื่อดูรายการที่ถูกลบในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="8ddb5-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="8ddb5-104">หลังจากที่คุณพบรายการที่ถูกลบ คุณใช้ cmdlet[คืนค่า-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps)เพื่อคืนค่ารายการเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="8ddb5-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="8ddb5-105">ดูรายละเอียดทั้งหมดใน[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="8ddb5-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="8ddb5-106">คุณต้องได้รับมอบหมายบทบาทการส่งออกการนําเข้ากล่องจดหมายก่อนจึงจะสามารถเรียกใช้ cmdlet นี้ได้</span><span class="sxs-lookup"><span data-stu-id="8ddb5-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="8ddb5-107">โปรดดู[ขอแก้ไขได้Items](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)สําหรับข้อมูลเพิ่มเติม.</span><span class="sxs-lookup"><span data-stu-id="8ddb5-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
