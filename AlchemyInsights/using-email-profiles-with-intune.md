---
title: การใช้โปรไฟล์อีเมลกับ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555759"
---
# <a name="using-email-profiles-with-intune"></a>การใช้โปรไฟล์อีเมลกับ Intun

Intunbe สามารถใช้เพื่อสร้างและปรับใช้โปรไฟล์อีเมลสําหรับไคลเอ็นต์อีเมลเนทีฟ (ในตัว) บนแพลตฟอร์มอุปกรณ์หลาย

สําหรับข้อมูลเกี่ยวกับข้อจํากัดบางอย่างที่เกี่ยวข้องกับโปรไฟล์อีเมล รวมถึงวิธีจัดการการมีอยู่ของโปรไฟล์ที่มีอยู่และวิธีการลบโปรไฟล์อีเมล โปรดดูที่[เพิ่มการตั้งค่าอีเมลไปยังอุปกรณ์ที่ใช้ Intun](https://docs.microsoft.com/intune/email-settings-configure)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีสร้างโปรไฟล์อีเมลสําหรับแต่ละแพลตฟอร์มอุปกรณ์ โปรดดู:

[การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่าอีเมล การตรวจสอบสิทธิ์ และการซิงโครไนซ์ใน Intun](https://docs.microsoft.com/intune/email-settings-android)  
[เพิ่มการตั้งค่าอีเมลสําหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni](https://docs.microsoft.com/intune/email-settings-ios)  
[การตั้งค่าส่วนกําหนดค่าอีเมลใน Microsoft Intun สําหรับอุปกรณ์ที่ใช้ Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[การตั้งค่าส่วนกําหนดค่าอีเมลสําหรับอุปกรณ์ที่ใช้ Windows 10 ใน Microsoft Intun](https://docs.microsoft.com/intune/email-settings-windows-10)

**ปัญหาการซิงค์ทั่วไป**

**KNOX บนโปรไฟล์อีเมล Android จะป้องกันไม่ให้ผู้ใช้ที่ติดต่อ ปฏิทิน และงาน จากการซิงค์ไปยังอุปกรณ์ของผู้ใช้**

KNOX บนโปรไฟล์อีเมลของ Android KNOX เสนอตัวเลือกสําหรับผู้ดูแลระบบในการตัดสินใจว่าจะซิงค์เนื้อหาประเภทใดไปยังอุปกรณ์โดยการตั้งค่าแต่ละเปิดใช้งาน

ถ้าการตั้งค่าสําหรับชนิดเนื้อหาใดๆ ถูกตั้งค่าเป็น**ไม่ได้กําหนดค่า**(ค่าเริ่มต้น) ชนิดเนื้อหานั้นจะไม่ซิงค์โดยอัตโนมัติ ผู้ใช้อาจเปิดใช้งานชนิดเนื้อหาที่ต้องการโดยตรงบนอุปกรณ์ด้วยตนเอง แต่การกําหนดค่านั้นถูกเขียนทับโดยการตั้งค่านโยบาย Intun

