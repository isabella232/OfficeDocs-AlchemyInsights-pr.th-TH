---
title: ใช้ข้อมูลMicrosoft Intuneพื้นฐานด้านความปลอดภัยเพื่อกําหนดค่าWindows 10อุปกรณ์
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971538"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>ใช้ข้อมูลMicrosoft Intuneพื้นฐานด้านความปลอดภัยในการกําหนดค่าWindows 10อุปกรณ์

ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย Intuns ช่วยปกป้องผู้ใช้และอุปกรณ์ ข้อมูลพื้นฐานWindowsการตั้งค่าพื้นฐานของกลุ่มที่กําหนดไว้ล่วงหน้าซึ่งใช้กลุ่มการตั้งค่าที่รู้จักและค่าเริ่มต้นที่แนะนาโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง คุณสามารถสร้างเทมเพลตที่ประกอบด้วยโปรไฟล์การกําหนดค่าอุปกรณ์ได้หลายโปรไฟล์ด้วยการสร้างโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัยใน Intuny

เมื่อคุณปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัยกับกลุ่มของผู้ใช้หรืออุปกรณ์ การตั้งค่าจะถูกใช้กับอุปกรณ์ที่เรียกใช้Windows 10 หรือเวอร์ชันที่ใหม่กว่า ตัวอย่างเช่น ข้อมูลพื้นฐานเกี่ยวกับการจัดการอุปกรณ์เคลื่อนที่ (MDM) ของ Microsoft โดยอัตโนมัติ (1) จะเปิดใช้งาน BitLocker เป็นไดรฟ์แบบถอดได้ (2) ต้องใช้รหัสผ่านเพื่อปลดล็อกอุปกรณ์ และ (3) ปิดใช้งานการรับรองความถูกต้องพื้นฐาน เมื่อค่าเริ่มต้นใช้ไม่ได้กับสภาพแวดล้อมของคุณ คุณสามารถปรับแต่งข้อมูลพื้นฐานเพื่อปรับใช้การตั้งค่าที่คุณต้องการได้

ข้อมูลพื้นฐานด้านความปลอดภัยยังช่วยสร้างเวิร์กโฟลว์ที่ปลอดภัยแบบ end-to-end ใน Microsoft 365อีกด้วย ต่อไปนี้เป็นประโยชน์บางอย่างของฟังก์ชันการฟังก์ชันนี้:
- ข้อมูลพื้นฐานด้านความปลอดภัยมีหลักปฏิบัติที่ดีที่สุดและข้อเสนอแนะเกี่ยวกับการตั้งค่าที่มีผลต่อความปลอดภัย เนื่องจาก Intuned เป็นคู่ค้าWindowsทีมรักษาความปลอดภัยสําหรับกลุ่มที่สร้างข้อมูลพื้นฐานสําหรับนโยบายกลุ่ม ข้อแนะนําเหล่านี้ยึดตามแนวทางที่ทึบและประสบการณ์การใช้งานที่ครอบคลุม
- ถ้าคุณยังใหม่กับ Intun1 และไม่แน่ใจว่าจะเริ่มที่ใด ข้อมูลพื้นฐานด้านความปลอดภัยจะช่วยให้คุณสร้างและปรับใช้โปรไฟล์ที่ปลอดภัยได้อย่างรวดเร็ว
- ถ้าคุณยังใช้นโยบายกลุ่มอยู่ การโยกย้ายไปยัง Intuned เพื่อวัตถุประสงค์ในการจัดการจะง่ายยิ่งขึ้นด้วยข้อมูลพื้นฐานด้านความปลอดภัย เนื่องจากข้อมูลพื้นฐานเหล่านี้มีอยู่แล้วภายใน Intuny และมีความสามารถในการจัดการที่ล้าสมัย

For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).