---
title: กําหนดค่าการตั้งค่าความเป็นส่วนตัวในMicrosoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090323"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>กําหนดค่าการตั้งค่าความเป็นส่วนตัวในMicrosoft Edge

ตามค่าเริ่มต้น ถ้ามีการปรับใช้Microsoft Edgeบนแพลตฟอร์มที่ไม่ใช่แพลตฟอร์ม Windows ข้อมูลการวินิจฉัยและข้อมูลไซต์จะไม่ส่งไปยังไมโครซอฟท์ อย่างไรก็ตาม หากมีการปรับใช้Microsoft Edgeใน Windows 10 ข้อมูลการวินิจฉัยและข้อมูลไซต์จะถูกส่งตามการตั้งค่าข้อมูลWindows[การวินิจฉัย](https://go.microsoft.com/fwlink/?linkid=2132472)ของผู้ใช้

เมื่อต้องการกําหนดMicrosoft Edgeจัดการการเก็บรวบรวมข้อมูลให้กับองค์กรของคุณ ให้ใช้นโยบายกลุ่มต่อไปนี้
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) จะเปิดการรายงานการใช้งานและข้อมูลที่เกี่ยวข้องกับการหยุดการหยุด
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470)ส่งข้อมูลไซต์ที่ใช้เพื่อปรับปรุงบริการของ Microsoftของคุณ

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [กําหนดค่าการตั้งค่า](https://go.microsoft.com/fwlink/?linkid=2132577)นโยบาย
