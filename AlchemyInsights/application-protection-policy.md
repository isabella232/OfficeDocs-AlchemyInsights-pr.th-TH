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
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969990"
---
# <a name="application-protection-policy"></a>นโยบายการป้องกันแอปพลิเคชัน

ถ้าคุณยังใหม่เกี่ยวกับนโยบายการป้องกันแอปพลิเคชัน (แอป) ให้ลองดู [ภาพรวมนโยบายการป้องกัน](https://docs.microsoft.com/intune/apps/app-protection-policy)แอป

เมื่อต้องการเริ่มต้นใช้งานแอป ให้ดู [วิธีการสร้างและกําหนดนโยบายการป้องกัน](https://docs.microsoft.com/intune/app-protection-policies)แอป

ข้อต้องการนโยบายการป้องกันแอปพลิเคชัน:

- ผู้ใช้มีสิทธิ์การใช้งาน Intun1 หรือ EMS
- ผู้ใช้อยู่ในกลุ่มที่เป้าหมายโดยนโยบายการป้องกันแอปพลิเคชัน
- ผู้ใช้ขององค์กรเท่านั้นที่ลงชื่อเข้าใช้แอปที่ได้รับการป้องกันบนอุปกรณ์
- แอปพลิเคชันได้ดําเนินการ[Intuned SDK](https://docs.microsoft.com/intune/app-sdk-get-started) For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

นโยบายจะมีผลบังคับใช้หลังจากที่ผู้ใช้ที่ตรงตามข้อต้องการข้างต้นลงชื่อเข้าใช้แอปที่เปิดใช้งาน Intun1 SDK The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy. 

สำหรับข้อมูลเพิ่มเติม ให้ดู:

[ถามที่ถามบ่อยเกี่ยวกับการแก้ไขปัญหาแอป/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[วิธีตรวจสอบการตั้งค่านโยบายการป้องกันแอปของคุณ](https://docs.microsoft.com/intune/app-protection-policies-validate)

[เข้าใจการตั้งเวลาการส่งอีเมลนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[วิธีการตรวจสอบนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies-monitor)