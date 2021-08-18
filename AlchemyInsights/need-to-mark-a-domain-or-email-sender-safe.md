---
title: ต้องการการเครื่องหมายโดเมนหรือผู้ส่งอีเมลว่าปลอดภัยหรือไม่
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
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319967"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>ต้องการการเครื่องหมายโดเมนหรือผู้ส่งอีเมลว่าปลอดภัยหรือไม่

- ไม่แ **นะให้ใช้รายชื่อ** ผู้ส่งที่ปลอดภัยเนื่องจากจะเปิดขึ้นเพื่อให้องค์กรของคุณเป็นสแปม การหลอกลวง และการปลอมแปลง
- อย่างไรก็ตาม หากมีข้อกําหนดทางธุรกิจ เราขอแ **นะFlow****[จดหมายกฎ](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** เหล่านี้ แนวทางของเราช่วยรับรองความถูกต้องของผู้ส่ง (การตรวจสอบการส่งโดเมนจะไม่ถูกปลอมแปลง) 
    **หมายเหตุ**: เราไม่แนะให้จัดการค่าบวกที่ผิดโดยใช้รายชื่อผู้ส่งที่ปลอดภัย เนื่องจากข้อยกเว้นของการกรองสแปมสามารถเปิดองค์กรของคุณให้การโจมตีด้านความปลอดภัยได้ ถ้าผู้ใช้ของคุณได้รับข้อความที่ระบุว่าเป็นสแปมหรืออีเมลขยะอย่างไม่ถูกต้อง ให้ **[รายงานข้อความและไฟล์ไปยัง Microsoft](https://protection.office.com/reportsubmission)**
- ตู้เซฟ ควรหลีกเลี่ยงผู้ส่งใน Outlook, รายชื่อผู้ส่งที่อนุญาต หรือรายการโดเมนที่อนุญาตในนโยบายการป้องกันสแปมเนื่องจากผู้ส่งข้ามสแปม การปลอมแปลง และการป้องกันการหลอกลวง และการรับรองความถูกต้องของผู้ส่งทั้งหมด (SPF, DKIM, DMARC) วิธีนี้ใช้ได้ดีที่สุดกับการทดสอบชั่วคราวเท่านั้น
- การตรวจสอบความถูกต้องของอีเมลที่เลี่ยงผ่านการประเมิน Antispam สามารถเสร็จสิ้นได้โดยการตรวจสอบส่วนหัวของข้อความ "X-Forsfront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN) ให้ดูที่ **[ส่วนหัวของ](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** ข้อความป้องกันสแปม
- เนื่องจาก Microsoft ต้องการให้ลูกค้าของเรามีความปลอดภัย [ตามค่าเริ่มต้น การแทนที่](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)ผู้เช่าบางอย่างจะไม่ถูกใช้กับมัลแวร์และฟิชชิ่งที่มีความเชื่อมั่นสูง การแทนที่เหล่านี้ ได้แก่: o รายชื่อผู้ส่งที่อนุญาตหรือรายการโดเมนที่อนุญาต (นโยบายการป้องกันสแปม) Outlook ตู้เซฟ รายชื่อผู้ส่ง o รายชื่อที่อนุญาต IP (การกรองการเชื่อมต่อ) 
- การแทนที่เพียงรายการเดียวที่อนุญาตให้ข้อความฟิชชิ่งความเชื่อมั่นสูงสามารถข้ามการกรองได้ Exchangeล้นจดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน) เมื่อต้องการใช้กฎของโฟลว์จดหมายเพื่อข้ามการกรอง ให้ดู ใช้กฎล.ล.ก. จดหมาย เพื่อตั้งค่า **[ระดับความเชื่อมั่นของสแปม (SCL) ใน](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** ข้อความ