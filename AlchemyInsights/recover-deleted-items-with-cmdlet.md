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
# <a name="recover-deleted-items-with-cmdlet"></a>กู้คืนรายการที่ถูกลบด้วย cmdlet

- ใช้ [cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูรายการที่ถูกลบในกล่องจดหมาย หลังจากที่คุณพบรายการที่ถูกลบ คุณใช้ cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) เพื่อคืนค่ารายการเหล่านั้น

- ดูรายละเอียดแบบเต็มใน[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)

- คุณต้องได้รับมอบหมายบทบาทนําเข้าส่งออกกล่องจดหมายก่อนที่คุณจะสามารถเรียกใช้ cmdlet นี้ โปรดดู [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูข้อมูลเพิ่มเติม
