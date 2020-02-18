---
title: ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091778"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>ไม่สามารถตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase

เมื่อพยายามตั้งค่าหรือดูนโยบาย AllowSelfServicePurchase คุณได้รับข้อความแจ้งความผิดพลาดต่อไปนี้:

*HandleError: ไม่สามารถเรียกนโยบายผลิตภัณฑ์ด้วย PolicyId ' AllowSelfServicePurchase ' ErrorMessage-การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*

ซึ่งอาจเกิดจากการขนส่งเลเยอร์ความปลอดภัย (TLS) รุ่นเก่า เมื่อต้องการเชื่อมต่อบริการ MSCommerce คุณจำเป็นต้องใช้ TLS ๑.๒หรือสูงกว่า  

ลองทำตามขั้นตอนต่อไปนี้เพื่อเปิดใช้งาน/ตั้งค่าโพรโทคอล TLS เพื่อ๑.๒ตรวจสอบและลองอีกครั้ง
 1. ที่พร้อมท์คำสั่ง PowerShell (PS C:\)ป้อนคำสั่งต่อไปนี้เพื่อตั้งค่าโพรโทคอล TLS รุ่น๑.๒:

    \[สุทธิ ServicePointManager]:: SecurityProtocol = \[สุทธิ SecurityProtocolType]::: Tls12

2. ตรวจสอบโพรโทคอล TLS (s) ที่ใช้กับคำสั่งต่อไปนี้:

    \[สุทธิ ServicePointManager]:: SecurityProtocol 

3. ลองรับหรือปรับปรุงคำสั่งตามที่จำเป็น

