---
title: แก้ไขปัญหาเกี่ยวกับอุปกรณ์ Windows 10 แบบออนบอร์ดจากระยะไกลไปยัง Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750045"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>แก้ไขปัญหาเกี่ยวกับอุปกรณ์ Windows 10 แบบออนบอร์ดจากระยะไกลไปยัง Microsoft Defender Advanced Threat Protection

ถ้าคุณสามารถเข้าถึงคอมพิวเตอร์ระยะไกล ได้ ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ดาวน์โหลด [เครื่องมือวินิจฉัยการเชื่อมต่อ](https://go.microsoft.com/fwlink/?linkid=2143466) ไคลเอ็นต์
2. แยกและเรียกใช้ MDATPAnalyzer.cmd
3. ค้นหาบันทึกการวินิจฉัยในโฟลเดอร์ MDATPClientAnalyzerResult ซึ่งเป็นโฟลเดอร์เดียวกันกับที่เครื่องมือวิเคราะห์ถูกดาวน์โหลด
4. เมื่อต้องการค้นหาปัญหาเกี่ยวกับการเชื่อมต่อหรือการตั้งค่าพร็อกซีอินเทอร์เน็ต ให้รีวิวไฟล์MDATPClientAnalyzer.txt

เมื่อต้องการเรียนรู้เพิ่มเติม[ดูปัญหาเกี่ยวกับเครื่องออนบอร์ด](https://go.microsoft.com/fwlink/?linkid=2143634)
