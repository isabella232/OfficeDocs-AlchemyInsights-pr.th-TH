---
title: กู้คืนรายการที่ถูกลบด้วย cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835830"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="39598-102">กู้คืนรายการที่ถูกลบด้วย cmdlet</span><span class="sxs-lookup"><span data-stu-id="39598-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="39598-103">ใช้ [cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูรายการที่ถูกลบในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="39598-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="39598-104">หลังจากที่คุณพบรายการที่ถูกลบ คุณใช้ cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) เพื่อคืนค่ารายการเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="39598-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="39598-105">ดูรายละเอียดแบบเต็มใน[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="39598-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="39598-106">คุณต้องได้รับมอบหมายบทบาทนําเข้าส่งออกกล่องจดหมายก่อนที่คุณจะสามารถเรียกใช้ cmdlet นี้</span><span class="sxs-lookup"><span data-stu-id="39598-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="39598-107">โปรดดู [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="39598-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
