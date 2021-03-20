---
title: ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoints
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901586"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoints

คุณอาจมีปัญหากับเครื่องออนบอร์ดลงในบริการ MDE ถ้าคุณสามารถเข้าถึงเครื่องของผู้ใช้ ปลายทาง ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ดาวน์โหลดเวอร์ชันล่าสุดของเครื่องมือวินิจฉัย[ตัววิเคราะห์ไคลเอ็นต์ MDE](https://aka.ms/betamdeanalyzer)
2. คลิกขวาที่ **MDEClientAnalyzer.cmd** แล้วเลือก 'เรียกใช้ในฐานะผู้ดูแลระบบ'
3. Follow any guidance suggested in **MDEClientAnalyzer.htm**.
4. ดูโฟลเดอร์ย่อยที่สร้างขึ้นที่ชื่อว่า **MDEClientAnalyzerResult** เพิ่มเติม
5. ถ้าต้องใช้แนวทางเพิ่มเติม ให้ติดต่อ [Microsoft Defender เพื่อรับการสนับสนุนเกี่ยวกับ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) จุดสิ้นสุด และMDEClientAnalyzerResult.zipไฟล์สําหรับการวิเคราะห์
