---
title: การใช้โปรไฟล์อีเมลกับ Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653307"
---
# <a name="using-email-profiles-with-intune"></a>การใช้โปรไฟล์อีเมลกับ Intune

Intune สามารถใช้ในการสร้างและปรับใช้โปรไฟล์อีเมลสำหรับไคลเอ็นต์อีเมลแบบดั้งเดิม (ภายใน) บนแพลตฟอร์มอุปกรณ์หลายเครื่อง

สำหรับข้อมูลเกี่ยวกับข้อจำกัดบางประการที่เกี่ยวข้องกับโปรไฟล์อีเมลรวมถึงวิธีการจัดการการแสดงตนของโปรไฟล์ที่มีอยู่และวิธีการเอาโปรไฟล์อีเมลให้ดู[เพิ่มการตั้งค่าอีเมลไปยังอุปกรณ์โดยใช้ Intune](https://docs.microsoft.com/intune/email-settings-configure)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการสร้างโปรไฟล์อีเมลสำหรับแต่ละแพลตฟอร์มอุปกรณ์ให้ดูที่:

[การตั้งค่าอุปกรณ์ Android เพื่อกำหนดค่าอีเมลการรับรองความถูกต้องและการซิงโครไนซ์ใน Intune](https://docs.microsoft.com/intune/email-settings-android)  
[เพิ่มการตั้งค่าอีเมลสำหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[การตั้งค่าโปรไฟล์อีเมลใน Microsoft Intune สำหรับอุปกรณ์ที่ใช้ Windows Phone ๘.๑](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[การตั้งค่าโปรไฟล์อีเมลสำหรับอุปกรณ์ที่ใช้ Windows 10 ใน Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**ปัญหาการซิงค์ทั่วไป**

**โปรไฟล์อีเมลของ KNOX บน Android จะป้องกันไม่ให้ผู้ติดต่อของผู้ใช้ปฏิทินและงานของผู้ใช้ได้รับการซิงค์กับอุปกรณ์ของผู้ใช้**

โปรไฟล์อีเมล knox ของ Android ใน Android จะมีตัวเลือกในการตัดสินใจเลือกชนิดเนื้อหาที่จะซิงค์ไปยังอุปกรณ์โดยการตั้งค่าแต่ละรายการที่จะเปิดใช้งาน

ถ้าการตั้งค่าสำหรับชนิดเนื้อหาใดๆถูกตั้งค่าเป็น **ไม่ได้กำหนดค่า** (ค่าเริ่มต้น) ชนิดเนื้อหานั้นจะไม่ถูกซิงค์โดยอัตโนมัติ ผู้ใช้อาจเปิดใช้งานชนิดเนื้อหาที่พวกเขาต้องการโดยตรงในอุปกรณ์ด้วยตนเองแต่การกำหนดค่าดังกล่าวจะถูกเขียนทับโดยการตั้งค่านโยบาย Intune และการหยุดการซิงค์สำหรับชนิดเนื้อหานั้น

