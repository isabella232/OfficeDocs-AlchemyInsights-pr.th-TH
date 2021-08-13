---
title: การใช้โปรไฟล์อีเมลด้วย Intuny
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919442"
---
# <a name="using-email-profiles-with-intune"></a>การใช้โปรไฟล์อีเมลด้วย Intuny

Intuny สามารถใช้ในการสร้างและปรับใช้โปรไฟล์อีเมลของไคลเอ็นต์อีเมลภายใน (ที่มีอยู่แล้วภายใน) บนแพลตฟอร์มอุปกรณ์หลายแพลตฟอร์มได้

For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intuny](https://docs.microsoft.com/intune/email-settings-configure).

ดูข้อมูลเพิ่มเติมเกี่ยวกับวิธีการสร้างโปรไฟล์อีเมลของแต่ละแพลตฟอร์มอุปกรณ์ที่:

[การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่าอีเมล การรับรองความถูกต้อง และการซิงโครไนซ์ใน Intun1](https://docs.microsoft.com/intune/email-settings-android)  
[เพิ่มการตั้งค่าอีเมลของอุปกรณ์ iOS และ iPadOS Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[การตั้งค่าโปรไฟล์อีเมลMicrosoft Intuneอุปกรณ์ที่ใช้ Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[การตั้งค่าโปรไฟล์อีเมลของอุปกรณ์ที่ใช้Windows 10ในMicrosoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**ปัญหาการซิงค์ทั่วไป**

**KNOX บนโปรไฟล์อีเมล Android จะป้องกันไม่ให้ที่ติดต่อ ปฏิทิน และงานของผู้ใช้ซิงค์กับอุปกรณ์ของผู้ใช้ไม่ได้**

โปรไฟล์อีเมล KNOX บน Android KNOX มีตัวเลือกให้ผู้ดูแลระบบตัดสินใจว่าจะซิงค์ชนิดเนื้อหาใดกับอุปกรณ์โดยการตั้งค่าแต่ละชนิดเพื่อเปิดใช้งาน

ถ้าการตั้งค่าของชนิดเนื้อหาใดๆ ถูกตั้งค่าเป็น **ไม่ได้กําหนดค่า** (ค่าเริ่มต้น) ชนิดเนื้อหานั้นจะไม่ถูกซิงค์โดยอัตโนมัติ ผู้ใช้อาจเปิดใช้งานชนิดเนื้อหาที่พวกเขาต้องการได้โดยตรงบนอุปกรณ์ด้วยตนเอง แต่การกําหนดค่าจะถูกเขียนทับโดยการตั้งค่านโยบาย Intun1 และการซิงค์จะหยุดการกําหนดค่าชนิดเนื้อหานั้น

