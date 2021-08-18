---
title: เหตุการณ์สดในYammerข้อผิดพลาดในการสร้าง
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
ms.openlocfilehash: eb1ef3712038827beafc8eb520f9793da5f357d728e8250c16d88a99b8b5fe20
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114947"
---
# <a name="live-events-in-yammer-creation-errors"></a>เหตุการณ์สดในYammerข้อผิดพลาดในการสร้าง

**Yammer การสร้างเหตุการณ์สด**

Yammerจะแสดงตัวเลือกในการสร้างเหตุการณ์สดตลอดเวลา ในบางกรณี ผู้ใช้อาจไม่ตรงตามข้อเบื้องต้นในการสร้างเหตุการณ์สด และได้รับข้อผิดพลาดเมื่อพวกเขาพยายามสร้างเหตุการณ์นั้น รายการด้านล่างครอบคลุมสาเหตุทั่วไปของปัญหานี้และมีวิธีการแก้ไขปัญหาให้กับผู้ใช้

**ใครสร้างเหตุการณ์สดได้**
- สิทธิ์การใช้งาน Office 365 Enterprise E1, E3 หรือ E5 หรือสิทธิ์การใช้งาน Office 365 A3 หรือ A5
- สิทธิ์ในการสร้างเหตุการณ์สดใน Microsoft Teamsศูนย์การจัดการ
- สิทธิ์ในการสร้างเหตุการณ์สดใน Microsoft Stream (เหตุการณ์ที่ผลิตโดยใช้แอปหรืออุปกรณ์การออกอากาศภายนอก)
- การเป็นสมาชิกทีมแบบเต็มในองค์กร (ไม่สามารถเป็นแขกหรือมาจากองค์กรอื่น)
- มีการเปิดการจัดตารางการประชุมส่วนตัว การแชร์หน้าจอ และการแชร์วิดีโอ IP ในนโยบายการประชุมทีม

**นโยบายการสร้างเหตุการณ์สด**

Yammerตามนโยบายเหตุการณ์สดที่ตั้งค่าในผู้Office 365ของคุณ for Stream ตามค่าเริ่มต้น ทุกคนในองค์กรของคุณสามารถสร้างเหตุการณ์สดได้ ผู้ดูแลระบบอาจ [เปลี่ยนแปลงการตั้งค่านี้อาจป้องกันไม่ให้ผู้ใช้สร้างเหตุการณ์](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)สดได้ It is important to check that users have permissions to create live events if they receive a policy error.
