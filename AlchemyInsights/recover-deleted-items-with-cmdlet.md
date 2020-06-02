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
# <a name="recover-deleted-items-with-cmdlet"></a>กู้คืนรายการที่ถูกลบด้วย cmdlet

- ใช้ cmdlet[รับการกู้คืนItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)เพื่อดูรายการที่ถูกลบในกล่องจดหมาย หลังจากที่คุณพบรายการที่ถูกลบ คุณใช้ cmdlet[คืนค่า-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps)เพื่อคืนค่ารายการเหล่านั้น

- ดูรายละเอียดทั้งหมดใน[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)

- คุณต้องได้รับมอบหมายบทบาทการส่งออกการนําเข้ากล่องจดหมายก่อนจึงจะสามารถเรียกใช้ cmdlet นี้ได้ โปรดดู[ขอแก้ไขได้Items](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)สําหรับข้อมูลเพิ่มเติม.
