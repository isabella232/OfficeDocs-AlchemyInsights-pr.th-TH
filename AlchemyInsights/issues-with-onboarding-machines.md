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
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054709"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoints

คุณอาจมีปัญหากับเครื่องออนบอร์ดกับบริการ MDE ถ้าคุณสามารถเข้าถึงเครื่องของผู้ใช้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ดาวน์โหลดเวอร์ชันล่าสุดของเครื่องมือวินิจฉัย[ตัววิเคราะห์ไคลเอ็นต์ MDE](https://aka.ms/betamdeanalyzer)
2. คลิกขวาที่ **MDEClientAnalyzer.cmd** แล้วเลือก 'เรียกใช้ในฐานะผู้ดูแลระบบ'
3. Follow any guidance suggested in **MDEClientAnalyzer.htm**.
4. For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.
5. ถ้าต้องใช้แนวทางเพิ่มเติม ให้ติดต่อ [ฝ่ายสนับสนุนของ Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) สําหรับจุดสิ้นสุดและMDEClientAnalyzerResult.zipไฟล์สําหรับการวิเคราะห์
