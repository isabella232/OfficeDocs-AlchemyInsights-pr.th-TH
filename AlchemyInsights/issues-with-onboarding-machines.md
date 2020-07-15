---
title: ปัญหาเกี่ยวกับเครื่องออนบอร์ด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141836"
---
# <a name="issues-with-onboarding-machines"></a>ปัญหาเกี่ยวกับเครื่องออนบอร์ด

คุณอาจมีปัญหากับเครื่องออนบอร์ดไปยังบริการ MDATP ถ้าคุณสามารถเข้าถึงเครื่องผู้ใช้ ให้ทําตามขั้นตอนเหล่านี้:

1. ดาวน์โหลดเครื่องมือการวินิจฉัย[ตัววิเคราะห์การเชื่อมต่อไคลเอ็นต์](https://aka.ms/mdatpanalyzer)
2. สารสกัดและเรียกใช้ MDATPAnalyzer.cmd.
3. ค้นหาล็อกการวินิจฉัยในโฟลเดอร์ที่เรียกว่า MDATPClientAnalyzerResult โฟลเดอร์เดียวกันที่เครื่องมือวิเคราะห์ถูกดาวน์โหลด
4. ตรวจสอบแฟ้มบันทึก MDATPClientAnalyzer.txt เพื่อค้นหาปัญหาการตั้งค่าการเชื่อมต่อหรือพร็อกซีอินเทอร์เน็ต