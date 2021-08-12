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
ms.openlocfilehash: b3f4f034d5d7486dafa1b5c1801a285b09a34644b811146f09f454fad9647833
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910673"
---
# <a name="recover-deleted-items-with-cmdlet"></a>กู้คืนรายการที่ถูกลบด้วย cmdlet

- ใช้ [cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูรายการที่ถูกลบในกล่องจดหมาย หลังจากที่คุณพบรายการที่ถูกลบ คุณใช้ cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) เพื่อคืนค่ารายการเหล่านั้น

- ดูรายละเอียดแบบเต็มใน[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)

- คุณต้องได้รับมอบหมายบทบาทนําเข้าส่งออกกล่องจดหมายก่อนที่คุณจะสามารถเรียกใช้ cmdlet นี้ โปรดดู [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูข้อมูลเพิ่มเติม
