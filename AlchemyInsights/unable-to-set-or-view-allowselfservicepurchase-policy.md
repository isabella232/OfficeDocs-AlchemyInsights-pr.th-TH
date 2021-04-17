---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826110"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase

เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้:

*HandleError : ไม่สามารถเรียกใช้นโยบายผลิตภัณฑ์ด้วย PolicyId 'AllowSelfServicePurchase', ErrorMessage - การเชื่อมต่อที่เกี่ยวข้องถูกปิด: เกิดข้อผิดพลาดที่ไม่คาดคิดขึ้นในการส่ง*

ซึ่งอาจเกิดจาก Transport Layer Security (TLS) เวอร์ชันที่เก่ากว่า เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณต้องใช้ TLS 1.2 หรือใหม่กว่า  

ลองขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS เป็น 1.2 ตรวจสอบ และลองอีกครั้ง
 1. ที่พร้อมท์สั่ง PowerShell (PS C: \) ใส่ค่าสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS เป็นเวอร์ชัน 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. ตรวจสอบโพรโทคอล TLS ที่ใช้อยู่ ด้วยสั่งต่อไปนี้:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. ลองสั่ง รับ หรือ อัปเดต ใหม่ตามต้องการ

