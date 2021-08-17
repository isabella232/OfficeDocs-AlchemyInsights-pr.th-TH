---
title: เปิดใช้งานการรับรองความถูกต้องและการแก้ไขปัญหา SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890453"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>เปิดใช้งานการรับรองความถูกต้องและการแก้ไขปัญหา SMTP

ถ้าคุณต้องการเปิดใช้งานการรับรองความถูกต้อง SMTP ให้กับกล่องจดหมาย หรือคุณได้รับข้อผิดพลาด "ไคลเอ็นต์ไม่ได้รับการรับรองความถูกต้อง", "การรับรองความถูกต้องไม่ส", หรือ "SmtpClientAuthentication" ที่มีรหัส 5.7.57 หรือ 5.7.3 หรือ 5.7.139 เมื่อคุณพยายามรีเลย์อีเมลโดยการรับรองความถูกต้องอุปกรณ์หรือแอปพลิเคชันด้วย Microsoft 365 ให้ปฏิบัติสามอย่างเหล่านี้เพื่อแก้ไขปัญหา:

1. ปิดใช้งาน [ค่าเริ่มต้นความปลอดภัยของ Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)โดยการสลับ **เปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย****เป็น** ไม่

    a. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบความปลอดภัย ผู้ดูแลการเข้าถึงตามเงื่อนไข หรือผู้ดูแลระบบส่วนกลาง<BR/>
    b. เรียกดู Azure Active Directory > **คุณสมบัติ**<BR/>
    c. เลือก **จัดการค่าเริ่มต้น** ความปลอดภัย<BR/>
    d. ตั้งค่า **เปิดใช้งานค่าเริ่มต้นความปลอดภัย****เป็น** ไม่<BR/>
    e. เลือกบันทึก

2. [เปิดใช้งานการส่ง SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) ไคลเอ็นต์บนกล่องจดหมายที่มีสิทธิ์การใช้งาน

    a. จากรายการศูนย์การจัดการ Microsoft 365 ให้ไปที่ **ผู้ใช้** ที่ใช้งานอยู่ แล้วเลือกผู้ใช้<BR/>
    b. ไปที่แท็บ จดหมาย และ **ภายใต้ แอปอีเมล** ให้เลือก **จัดการแอป** อีเมล<BR/>
    d. ตรวจสอบให้แน่ใจว่า **มีการตรวจสอบ SMTP** ที่ได้รับการรับรองความถูกต้อง (เปิดใช้งาน)<BR/>
    e. เลือก **บันทึก** การเปลี่ยนแปลง<BR/>

3. [ปิดใช้งานการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) บนกล่องจดหมายที่มีสิทธิ์การใช้งาน

    a. ไปที่ตัวเลือก ศูนย์การจัดการ Microsoft 365 และในเมนูการนําทางด้านซ้าย ให้เลือก  >  **ผู้ใช้ที่ใช้งานอยู่**<BR/>
    b. เลือก **การรับรองความถูกต้องโดยใช้หลาย** ปัจจัย<BR/>
    c. เลือกผู้ใช้และ **ปิดใช้งานการรับรองความถูกต้องโดยใช้หลาย** ปัจจัย<BR/>
