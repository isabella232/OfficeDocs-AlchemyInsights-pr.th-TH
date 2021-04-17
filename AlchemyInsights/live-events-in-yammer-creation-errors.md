---
title: เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825534"
---
# <a name="live-events-in-yammer-creation-errors"></a>เหตุการณ์สดในข้อผิดพลาดในการสร้าง Yammer

**การสร้างเหตุการณ์สดของ Yammer**

Yammer จะแสดงตัวเลือกในการสร้างเหตุการณ์สดตลอดเวลา ในบางกรณี ผู้ใช้อาจไม่ตรงตามข้อเบื้องต้นในการสร้างเหตุการณ์สด และได้รับข้อผิดพลาดเมื่อพวกเขาพยายามสร้างเหตุการณ์นั้น รายการด้านล่างครอบคลุมสาเหตุทั่วไปของปัญหานี้และมีวิธีการแก้ไขปัญหาให้กับผู้ใช้

**ใครสามารถสร้างเหตุการณ์สดได้**
- สิทธิ์การใช้งาน Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5
- สิทธิ์ในการสร้างเหตุการณ์สดในศูนย์การจัดการ Microsoft Teams
- สิทธิ์ในการสร้างเหตุการณ์สดใน Microsoft Stream (เหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)
- การเป็นสมาชิกทีมแบบเต็มในองค์กร (ไม่สามารถเป็นแขกหรือมาจากองค์กรอื่น)
- มีการเปิดการจัดตารางการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP ในนโยบายการประชุมทีม

**นโยบายการสร้างเหตุการณ์สด**

Yammer จะเป็นไปตามนโยบายเหตุการณ์สดที่ตั้งค่าในผู้เช่า Office 365 ของคุณเพื่อสตรีม ตามค่าเริ่มต้น ทุกคนในองค์กรของคุณสามารถสร้างเหตุการณ์สดได้ ผู้ดูแลระบบอาจ [เปลี่ยนแปลงการตั้งค่านี้อาจป้องกันไม่ให้ผู้ใช้สร้างเหตุการณ์](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)สดได้ It is important to check that users have permissions to create live events if they receive a policy error.
