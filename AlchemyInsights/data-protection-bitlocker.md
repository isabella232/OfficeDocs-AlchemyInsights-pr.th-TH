---
title: DataProtection-Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731258"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>การเปิดใช้งานการเข้ารหัสลับ Bitlocker ด้วย Intune

 นโยบายการป้องกันจุดสิ้นสุดของ Intune สามารถใช้เพื่อกำหนดการตั้งค่าการเข้ารหัสลับของ Bitlocker สำหรับอุปกรณ์ Windows สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การตั้งค่า Windows 10 (และเวอร์ชันที่ใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)
 
คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย Bitlocker โดยอัตโนมัติซึ่งจะถูกทริกเกอร์โดยไม่มีแอปพลิเคชันของนโยบาย MDM การทำเช่นนี้อาจส่งผลกระทบต่อการใช้นโยบายถ้าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้นถูกกำหนดค่า ดูคำถามที่ถามบ่อยต่อไปนี้สำหรับรายละเอียดเพิ่มเติม
 
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาของ bitlocker ให้ดู[ที่แก้ไขปัญหานโยบาย bitlocker ใน Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**คำถามที่ถามบ่อย**

 Q: รุ่นของการเข้ารหัสลับอุปกรณ์ของ Windows ที่สนับสนุนโดยใช้นโยบายการป้องกันจุดสิ้นสุดหรือไม่<br>
 A: การตั้งค่าในนโยบายการป้องกันจุดสิ้นสุดของ Intune จะถูกนำไปใช้โดยใช้[CSP ของ Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) ไม่ใช่เวอร์ชันหรือรุ่นทั้งหมดของ Windows สนับสนุน Bitlocker CSP <br><br>
      ในตอนนี้ Windows รุ่นต่อไปนี้ได้รับการสนับสนุน: Enterprise, Education, Mobile, mobile Enterprise และ Professional (รุ่น๑๘๐๙และเวอร์ชันที่ใหม่กว่า)
 
Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับการเข้ารหัสลับและความแรงของการเข้ารหัส (XTS-AES-๑๒๘) จะนำนโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ด้วยการตั้งค่าใหม่อีกครั้ง<br>
A: ไม่ใช่ เมื่อต้องการนำการตั้งค่าการเข้ารหัสใหม่ไปใช้ไดรฟ์จะต้องถอดรหัสลับก่อน<br><br>
**หมายเหตุ:** สำหรับอุปกรณ์ที่กำลังลงทะเบียนกับ Autopilot การเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นระหว่าง OOBE จะไม่ทริกเกอร์จนกว่าจะมีการประเมินนโยบาย Intune จนกว่าจะมีการประเมินนโยบายของ Intune ซึ่งจะทำให้การตั้งค่านโยบายถูกนำไปใช้แทนที่ค่าเริ่มต้นของระบบปฏิบัติการ
 
Q: ถ้าอุปกรณ์ได้รับการเข้ารหัสลับเป็นผลลัพธ์ของแอปพลิเคชัน Intune ของ Intune จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่<br>
A: การลบนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ทำให้เกิดการถอดรหัสลับของไดรฟ์ที่ได้รับการกำหนดค่า
 
Q: เหตุใดนโยบายการปฏิบัติตามนโยบายของ Intune ของ Intune จึงแสดงว่าอุปกรณ์ของฉันไม่ได้เปิดใช้งาน Bitlocker แม้ว่าจะเป็นใช่หรือไม่<br>
A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบายของ Intune ที่ใช้ไคลเอ็นต์ Windows อุปกรณ์สถานภาพรับรอง (DHA) ไคลเอ็นต์นี้จะวัดสถานะอุปกรณ์ในเวลาเริ่มต้นเท่านั้น ดังนั้นถ้าอุปกรณ์ยังไม่ได้รับการรีบูตเนื่องจากการเข้ารหัสลับด้วย Bitlocker เสร็จสมบูรณ์บริการของไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ที่กำลังถูกใช้งานอยู่
 
 