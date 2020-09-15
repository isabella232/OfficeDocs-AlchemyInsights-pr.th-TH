---
title: ข้อผิดพลาดของทีม4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700222"
---
# <a name="4c7-error-in-microsoft-teams"></a>ข้อผิดพลาด4c7 ในทีม Microsoft

ข้อผิดพลาดนี้เกิดขึ้นเนื่องจากทีม Microsoft จำเป็นต้องมีการรับรองความถูกต้องของฟอร์ม เมื่อคุณปรับใช้บริการสหพันธรัฐไดเรกทอรีที่ใช้งานอยู่ (AD FS) จะไม่มีการเปิดใช้งานการรับรองความถูกต้องของฟอร์มสำหรับอินทราเน็ตตามค่าเริ่มต้น ถ้าการรับรองความถูกต้องแบบรวมของ Windows ล้มเหลวคุณจะได้รับพร้อมท์ให้ลงชื่อเข้าใช้โดยใช้การรับรองความถูกต้องของฟอร์ม

เมื่อต้องการแก้ไขปัญหานี้ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้สแน็ปอิน AD FS Microsoft Management Console (MMC) บนคอมพิวเตอร์ที่มีสำเนาของ Active Directory ภายในเครื่อง เมื่อต้องการทำเช่นนี้ให้ทำตามขั้นตอนต่อไปนี้: 

1. ในบานหน้าต่างนำทางให้เรียกดู**นโยบายการรับรองความถูกต้อง**
2. ภายใต้**การดำเนินการ**ในบานหน้าต่างรายละเอียดให้เลือก**แก้ไขการรับรองความถูกต้องหลักส่วนกลาง**
3. บนแท็บ**อินทราเน็ต**ให้เลือกการ**รับรองความถูกต้องของฟอร์ม**
4. เลือก **ตกลง** (หรือ **นำไปใช้**)