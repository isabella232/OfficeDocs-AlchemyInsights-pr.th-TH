---
title: แก้ไขปัญหาตัวจัดคิวงานพิมพ์แล้ว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911357"
---
# <a name="print-spooler-issue-is-resolved"></a>แก้ไขปัญหาตัวจัดคิวงานพิมพ์แล้ว

ถ้าอุปกรณ์ของคุณได้รับการอัปเดตด้วย Windows 10 **OS รุ่น 19041.329** คุณอาจพบปัญหาที่เครื่องพิมพ์บางเครื่องล้มเหลวในการพิมพ์   ตัวจัดคิวงานพิมพ์อาจแสดงข้อผิดพลาดหรือปิดโดยไม่คาดคิดเมื่อพยายามพิมพ์ และไม่มีผลลัพธ์มาจากเครื่องพิมพ์ที่ได้รับผลกระทบ ปัญหานี้ได้รับการแก้ไขแล้วใน OS รุ่น **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**การตรวจสอบอย่างต่อเนื่อง**

ไฟล์ Local Security Authority Subsystem Service (LSASS) (**Isass.exe**) อาจล้มเหลวบนบางอุปกรณ์ที่มีข้อความแสดงข้อผิดพลาด "กระบวนการระบบที่ร้ายแรง C:\WINDOWS\system32\Isass.exe ล้มเหลวด้วยรหัสสถานะ c0000008 เครื่องต้องเริ่มระบบใหม่ในขณะนี้"  **Microsoft จะแก้ไขปัญหาและจะมอบการอัปเดตในรุ่นที่จะเกิดขึ้น**

For more information, please check out [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).