---
title: นโยบายการป้องกันแอปพลิเคชัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716912"
---
# <a name="application-protection-policy"></a>นโยบายการป้องกันแอปพลิเคชัน

ถ้าคุณกำลังใช้นโยบายการคุ้มครองแอปพลิเคชันใหม่ (แอป) ให้ดู[ภาพรวมนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/apps/app-protection-policy)

เมื่อต้องการเริ่มต้นใช้งานแอปให้ดู[ที่วิธีการสร้างและกำหนดนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies)

ข้อกำหนดนโยบายการป้องกันแอปพลิเคชัน:

- ผู้ใช้มีสิทธิ์การใช้งาน Intune หรือ EMS
- ผู้ใช้เป็นสมาชิกของกลุ่มที่มีการกำหนดเป้าหมายโดยนโยบายการป้องกันแอปพลิเคชัน
- มีเพียงผู้ใช้ขององค์กรเดียวเท่านั้นที่ลงชื่อเข้าใช้แอปที่ได้รับการป้องกันบนอุปกรณ์
- แอปพลิเคชันได้นำไปใช้กับ[INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started) สำหรับรายการแอปที่สนับสนุน SDK ให้ดูที่ [แอป Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps)ที่ได้รับการป้องกัน

นโยบายจะนำไปใช้หลังจากที่ผู้ใช้ที่ตรงตามข้อกำหนดข้างต้นลงในแอป Intune SDK ที่เปิดใช้งานของ Intune วิธีที่ง่ายที่สุดในการตรวจสอบว่ามีการนำนโยบายไปใช้หรือไม่โดยต้องการให้ผู้ใช้ตั้งค่า pin ในนโยบาย 

สำหรับข้อมูลเพิ่มเติม ให้ดูที่

[คำถามที่ถามบ่อยเกี่ยวกับการแก้ไขปัญหาของแอป/แหม่ม](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[วิธีตรวจสอบการตั้งค่านโยบายการป้องกันแอปของคุณ](https://docs.microsoft.com/intune/app-protection-policies-validate)

[ทำความเข้าใจเกี่ยวกับการกำหนดเวลาการส่งนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[วิธีการตรวจสอบนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies-monitor)