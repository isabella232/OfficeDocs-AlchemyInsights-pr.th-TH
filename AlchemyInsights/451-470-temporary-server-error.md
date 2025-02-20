---
title: 451 4.7.0 ข้อผิดพลาดของเซิร์ฟเวอร์ชั่วคราว โปรดลองอีกครั้งในภายหลัง PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812592"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 ข้อผิดพลาดของเซิร์ฟเวอร์ชั่วคราว โปรดลองอีกครั้งในภายหลัง PRX4

คุณอาจพบปัญหาขณะส่งอีเมลผ่าน Smarthost "smtp.office365.com" โดยใช้วิธีส่งไคลเอ็นต์ SMTP และรับข้อผิดพลาด: "451 4.7.0 ข้อผิดพลาดเซิร์ฟเวอร์ชั่วคราว โปรดลองอีกครั้งในภายหลัง PRX4 เป็นส่วนใหญ่ชั่วคราว" 

ตรวจสอบให้แน่ใจว่าคุณไม่ได้ใช้กล่องจดหมายที่แชร์ในการส่งไคลเอ็นต์ SMTP เนื่องจากวิธีการส่งไคลเอ็นต์ SMTP ต้องใช้กล่องจดหมายที่มีสิทธิ์การใช้งานในการส่งจดหมาย อย่างไรก็ตาม ถ้าคุณไม่ได้ใช้กล่องจดหมายที่แชร์ แต่ยังคงพบปัญหา ให้ตรวจสอบดังต่อไปนี้:

1. เปิดใช้งานการส่ง SMTP ไคลเอ็นต์บนกล่องจดหมายที่มีสิทธิ์การใช้งานที่ใช้โดยการเรียกใช้สั่ง PowerShell นี้:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. ไปที่ศูนย์การจัดการ Microsoft 365 >**ผู้ใช้** ที่ใช้งานอยู่ แล้วเลือกผู้ใช้
    1. ไปที่แท็บ จดหมาย > **อีเมล >** **เลือก จัดการแอป** อีเมล 
    1. ตรวจสอบให้แน่ใจว่า **เลือกการตั้งค่า SMTP** ที่ได้รับการรับรองความถูกต้อง (เปิดใช้งาน)
    1. เลือก **บันทึก** การเปลี่ยนแปลง
    
    เมื่อต้องการเปิดใช้งานการรับรองความถูกต้องของ SMTP ให้กับทั้งองค์กร ให้เรียกใช้การสั่งนี้:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **หมายเหตุ**: ด้วยเหตุผลด้านความปลอดภัย เราแนะนนะให้คุณเปิดใช้งานการรับรองความถูกต้องของ SMTP เฉพาะกล่องจดหมายที่ใช้อยู่เท่านั้น การตั้งค่าระดับผู้ใช้จะแทนที่การตั้งค่าระดับองค์กร

2. ปิดใช้งานค่าเริ่มต้นความปลอดภัยของ Azure โดยการสลับ เปิดใช้งาน **ค่าเริ่มต้นด้านความปลอดภัยเป็น****ไม่ใช่**:

    1. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบความปลอดภัย ผู้ดูแลการเข้าถึงตามเงื่อนไข หรือผู้ดูแลระบบส่วนกลาง
    1. เรียกดู Azure Active Directory >**  คุณสมบัติ** แล้วเลือก **จัดการค่าเริ่มต้น** ด้านความปลอดภัย
    1. ตั้งค่า **การสลับ เปิดใช้งานค่าเริ่มต้น** ความปลอดภัย **เป็น** ไม่ใช่
    1. เลือกบันทึก

3. ปิดใช้งานการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA) บนกล่องจดหมายที่มีสิทธิ์การใช้งานที่ใช้อยู่

    1. ไปที่ตัวเลือก ศูนย์การจัดการ Microsoft 365 และในเมนูการนําทางด้านซ้าย ให้เลือก  >  **ผู้ใช้ผู้ใช้** ที่ใช้งานอยู่
    1. บนหน้า **ผู้ใช้ที่ใช้งานอยู่** ให้เลือก **การรับรองความถูกต้องโดยใช้หลาย** ปัจจัย
    1. เลือกผู้ใช้ และปิดใช้งาน **การรับรองความถูกต้องโดยใช้หลาย** ปัจจัย

