---
title: การซื้อแบบบริการตนเองของ PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091777"
---
# <a name="self-service-purchase-of-powershell"></a>การซื้อแบบบริการตนเองของ PowerShell

เมื่อต้องการใช้โมดูล PowerShell MSCommerce คุณจำเป็นต้องติดตั้งบนอุปกรณ์ Windows 10 ด้วย TLS ๑.๒ (ที่ต้องการสิทธิ์ของผู้ดูแลระบบภายในเครื่อง)  นำเข้าและเชื่อมต่อกับโมดู MSCommerce  เมื่อได้รับพร้อมท์ให้เข้าสู่ระบบคุณจะต้องใช้ข้อมูลประจำตัวของบทบาทผู้ดูแลระบบในการเรียกเก็บเงินสากล  

ถ้าคุณไม่มี TLS ๑.๒คุณอาจได้รับข้อผิดพลาดต่อไปนี้เมื่อพยายามรับหรือปรับปรุงนโยบาย:

*ErrorMessage-การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*



