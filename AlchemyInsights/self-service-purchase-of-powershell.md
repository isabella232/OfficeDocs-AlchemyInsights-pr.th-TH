---
title: การซื้อแบบบริการตนเองของ PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739989"
---
# <a name="self-service-purchase-of-powershell"></a>การซื้อแบบบริการตนเองของ PowerShell

เมื่อต้องการใช้โมดูล PowerShell ของ MSCommerce คุณจำเป็นต้องติดตั้งบนอุปกรณ์ Windows 10 ที่มี TLS ๑.๒ (ต้องมีสิทธิ์ผู้ดูแลระบบภายในเครื่อง)  นำเข้าและเชื่อมต่อกับโมดู MSCommerce  เมื่อได้รับพร้อมท์ให้เข้าสู่ระบบคุณจะต้องใช้ข้อมูลประจำตัวของบทบาทผู้ดูแลระบบส่วนกลางหรือผู้ดูแลการเรียกเก็บเงิน  

ถ้าคุณไม่มี TLS ๑.๒คุณอาจได้รับข้อผิดพลาดต่อไปนี้เมื่อพยายามที่จะรับหรืออัปเดการนโยบาย:

*ErrorMessage-การเชื่อมต่อขีดเส้นใต้ถูกปิด: มีข้อผิดพลาดที่ไม่คาดคิดเกิดขึ้นในการส่ง*



