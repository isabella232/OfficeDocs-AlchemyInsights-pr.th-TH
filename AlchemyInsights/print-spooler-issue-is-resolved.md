---
title: ปัญหาตัวจัดคิวงานพิมพ์ได้รับการแก้ไขแล้ว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088527"
---
# <a name="print-spooler-issue-is-resolved"></a>ปัญหาตัวจัดคิวงานพิมพ์ได้รับการแก้ไขแล้ว

หากอุปกรณ์ของคุณได้รับการอัปเดตด้วย Windows 10 **OS Build 19041.329**คุณอาจสังเกตเห็นปัญหาที่ทําให้เครื่องพิมพ์บางเครื่องไม่สามารถพิมพ์ได้ ตัวจัดคิวงานพิมพ์อาจแสดงข้อผิดพลาด หรือปิดโดยไม่คาดคิดเมื่อพยายามพิมพ์ และไม่มีผลลัพธ์ใดมาจากเครื่องพิมพ์ที่ได้รับผลกระทบ ปัญหานี้แก้ไขได้ในระบบปฏิบัติการรุ่น**19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**การสืบสวนอย่างต่อเนื่อง**

แฟ้มบริการระบบย่อย (LSASS)** (Isass.exe)** อาจล้มเหลวบนอุปกรณ์บางอย่างที่มีข้อความแสดงข้อผิดพลาด "กระบวนการระบบที่สําคัญ C:\WINDOWS\system32\Isass.exe ล้มเหลวด้วยรหัสสถานะ c0000008 เครื่องต้องเริ่มต้นใหม่"  **Microsoft กําลังทํางานเกี่ยวกับความละเอียด และจะมีการปรับปรุงในรุ่นต่อไป**

สําหรับข้อมูลเพิ่มเติม โปรดตรวจสอบ[ปัญหา Windows 10 เวอร์ชัน 2004 ที่ทราบ](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)