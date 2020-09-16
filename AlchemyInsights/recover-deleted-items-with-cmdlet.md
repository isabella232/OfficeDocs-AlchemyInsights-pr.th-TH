---
title: กู้คืนรายการที่ถูกลบด้วย cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741322"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="1dcf4-102">กู้คืนรายการที่ถูกลบด้วย cmdlet</span><span class="sxs-lookup"><span data-stu-id="1dcf4-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="1dcf4-103">ใช้ cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูรายการที่ถูกลบในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="1dcf4-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="1dcf4-104">หลังจากที่คุณพบรายการที่ถูกลบแล้วคุณสามารถใช้ cmdlet การ [คืนค่า-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) เพื่อคืนค่าได้</span><span class="sxs-lookup"><span data-stu-id="1dcf4-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="1dcf4-105">ดูรายละเอียดทั้งหมดในการ[รับ RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1dcf4-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="1dcf4-106">คุณจำเป็นต้องได้รับมอบหมายบทบาทการส่งออกการนำเข้ากล่องจดหมายก่อนที่คุณจะสามารถเรียกใช้ cmdlet นี้ได้</span><span class="sxs-lookup"><span data-stu-id="1dcf4-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="1dcf4-107">โปรดดูข้อมูลเพิ่มเติม [ได้ที่ RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1dcf4-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
