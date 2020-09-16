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
# <a name="recover-deleted-items-with-cmdlet"></a>กู้คืนรายการที่ถูกลบด้วย cmdlet

- ใช้ cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) เพื่อดูรายการที่ถูกลบในกล่องจดหมาย หลังจากที่คุณพบรายการที่ถูกลบแล้วคุณสามารถใช้ cmdlet การ [คืนค่า-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) เพื่อคืนค่าได้

- ดูรายละเอียดทั้งหมดในการ[รับ RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)

- คุณจำเป็นต้องได้รับมอบหมายบทบาทการส่งออกการนำเข้ากล่องจดหมายก่อนที่คุณจะสามารถเรียกใช้ cmdlet นี้ได้ โปรดดูข้อมูลเพิ่มเติม [ได้ที่ RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) สำหรับข้อมูลเพิ่มเติม
