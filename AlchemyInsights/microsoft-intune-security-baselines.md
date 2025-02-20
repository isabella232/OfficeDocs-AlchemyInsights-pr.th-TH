---
title: ใช้Microsoft Intuneพื้นฐานด้านความปลอดภัยเพื่อกําหนดค่าWindows 10ต่างๆ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332004"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>ใช้Microsoft Intuneพื้นฐานด้านความปลอดภัยเพื่อกําหนดค่าWindows 10ต่างๆ

ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย Intuns ช่วยปกป้องผู้ใช้และอุปกรณ์ ข้อมูลพื้นฐานWindowsการตั้งค่าพื้นฐานที่กําหนดไว้ล่วงหน้าซึ่งใช้กลุ่มการตั้งค่าที่รู้จักและค่าเริ่มต้นที่แนะนาโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง คุณสามารถสร้างเทมเพลตที่ประกอบด้วยโปรไฟล์การกําหนดค่าอุปกรณ์ได้หลายโปรไฟล์ด้วยการสร้างโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัยใน Intuny

เมื่อคุณปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัยกับกลุ่มของผู้ใช้หรืออุปกรณ์ การตั้งค่าจะถูกใช้กับอุปกรณ์ที่เรียกใช้Windows 10 หรือใหม่กว่า ตัวอย่างเช่น ข้อมูลพื้นฐานเกี่ยวกับการจัดการอุปกรณ์เคลื่อนที่ (MDM) ของ Microsoft จะเปิดใช้งาน BitLocker บนไดรฟ์แบบถอดได้โดยอัตโนมัติ ต้องการรหัสผ่านเพื่อปลดล็อกอุปกรณ์ และปิดใช้งานการรับรองความถูกต้องพื้นฐาน เมื่อค่าเริ่มต้นใช้ไม่ได้กับสภาพแวดล้อมของคุณ คุณสามารถปรับแต่งข้อมูลพื้นฐานเพื่อปรับใช้การตั้งค่าที่คุณต้องการได้

ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยยังช่วยสร้างเวิร์กโฟลว์ที่ปลอดภัยแบบ end-to-end ใน Microsoft 365อีกด้วย ข้อมูลพื้นฐานด้านความปลอดภัยมีหลักปฏิบัติที่ดีที่สุดและข้อเสนอแนะเกี่ยวกับการตั้งค่าที่มีผลต่อความปลอดภัย Intun1 เป็นคู่ค้าWindowsทีมรักษาความปลอดภัยใหม่ที่สร้างข้อมูลพื้นฐานสําหรับนโยบายกลุ่ม ดังนั้นข้อแนะนําเหล่านี้ยึดตามแนวทางที่ทึบและประสบการณ์การใช้งานที่ครอบคลุม

ถ้าคุณยังใหม่กับ Intun1 และไม่แน่ใจเกี่ยวกับจุดเริ่มต้น การรักษาความปลอดภัยพื้นฐานจะช่วยให้คุณสร้างและปรับใช้โปรไฟล์ที่ปลอดภัยได้อย่างรวดเร็ว ถ้าคุณใช้นโยบายกลุ่มในปัจจุบัน การโยกย้ายไปยัง Intuned เพื่อวัตถุประสงค์ในการจัดการจะง่ายขึ้นมากด้วยข้อมูลพื้นฐานด้านความปลอดภัยเนื่องจากข้อมูลเหล่านั้นมีอยู่แล้วใน Intuny และมีความสามารถในการจัดการที่ล้่สุด

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู Windowsพื้นฐานความปลอดภัยและ](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)[การจัดการอุปกรณ์เคลื่อน](https://docs.microsoft.com/windows/client-management/mdm/)ที่

