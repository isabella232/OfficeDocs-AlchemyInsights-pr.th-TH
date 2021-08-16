---
title: แก้ไขปัญหาจากระยะไกลด้วยการออนบอร์ดWindows 10ไปยัง Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034053"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>แก้ไขปัญหาจากระยะไกลด้วยการออนบอร์ดWindows 10ไปยัง Microsoft Defender Advanced Threat Protection

ถ้าคุณสามารถเข้าถึงคอมพิวเตอร์ระยะไกลได้ ให้ปฏิบัติตามขั้นตอนเหล่านี้

1. ดาวน์โหลด [เครื่องมือวินิจฉัยการเชื่อมต่อ](https://go.microsoft.com/fwlink/?linkid=2143466) ไคลเอ็นต์
2. แยกและเรียกใช้ MDATPAnalyzer.cmd
3. ค้นหาบันทึกการวินิจฉัยในโฟลเดอร์ MDATPClientAnalyzerResult ซึ่งเป็นโฟลเดอร์เดียวกันกับที่ดาวน์โหลดเครื่องมือตัววิเคราะห์
4. เมื่อต้องการค้นหาปัญหาเกี่ยวกับการตั้งค่าการเชื่อมต่อหรือพร็อกซีอินเทอร์เน็ต ให้รีวิวไฟล์บันทึกMDATPClientAnalyzer.txt

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู ปัญหาเกี่ยวกับเครื่องออนบอร์ด](https://go.microsoft.com/fwlink/?linkid=2143634)
