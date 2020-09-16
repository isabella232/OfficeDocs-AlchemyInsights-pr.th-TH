---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735218"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase

เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณจะได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้:

*HandleError: ล้มเหลวในการเรียกใช้นโยบายผลิตภัณฑ์ด้วย PolicyId ' AllowSelfServicePurchase ' ErrorMessage-การเชื่อมต่อขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*

การทำเช่นนี้อาจเป็นเพราะเวอร์ชันที่เก่ากว่าของความปลอดภัยของชั้นการขนส่ง (TLS) เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณจำเป็นต้องใช้ TLS ๑.๒หรือสูงกว่า  

ให้ลองทำตามขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS ไปยัง๑.๒ตรวจสอบแล้วลองอีกครั้ง
 1. ที่พร้อมท์คำสั่ง PowerShell (PS C: \) ใส่คำสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS เป็นเวอร์ชัน๑.๒:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. ตรวจสอบว่าโพรโทคอล TLS ถูกใช้งานอยู่ด้วยคำสั่งต่อไปนี้:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. ลองใช้คำสั่งรับหรืออัปเดตใหม่ตามต้องการ

