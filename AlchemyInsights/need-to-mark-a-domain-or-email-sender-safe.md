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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792151"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>ต้องการการเครื่องหมายโดเมนหรือผู้ส่งอีเมลว่าปลอดภัยหรือไม่

- ไม่แ **นะให้ใช้รายชื่อ** ผู้ส่งที่ปลอดภัยเนื่องจากจะเปิดขึ้นเพื่อให้องค์กรของคุณเป็นสแปม การหลอกลวง และการปลอมแปลง
- อย่างไรก็ตาม หากมีข้อกําหนดทางธุรกิจ เราขอแนะนนะ **ให้** ใช้ **[กฎล](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .จดหมาย แนวทางของเราช่วยรับรองความถูกต้องของผู้ส่ง (การตรวจสอบการส่งโดเมนจะไม่ถูกปลอมแปลง) **หมายเหตุ**: เราไม่แนะให้จัดการค่าบวกที่ผิดโดยใช้รายชื่อผู้ส่งที่ปลอดภัย เนื่องจากข้อยกเว้นของการกรองสแปมสามารถเปิดองค์กรของคุณให้การโจมตีด้านความปลอดภัยได้ ถ้าผู้ใช้ของคุณได้รับข้อความถูกระบุว่าเป็นสแปมหรืออีเมลขยะอย่างไม่ถูกต้อง โปรด **[รายงานข้อความและไฟล์ไปยัง Microsoft](https://protection.office.com/reportsubmission)**
- ควรหลีกเลี่ยงผู้ส่งที่ปลอดภัยใน Outlook, รายชื่อผู้ส่งที่ได้รับอนุญาต หรือรายการโดเมนที่อนุญาตในนโยบายการป้องกันสแปม เนื่องจากผู้ส่งข้ามสแปม การปลอมแปลง และการป้องกันการหลอกลวงและการรับรองความถูกต้องของผู้ส่งทั้งหมด (SPF, DKIM, DMARC) วิธีนี้ใช้ได้ดีที่สุดกับการทดสอบชั่วคราวเท่านั้น
