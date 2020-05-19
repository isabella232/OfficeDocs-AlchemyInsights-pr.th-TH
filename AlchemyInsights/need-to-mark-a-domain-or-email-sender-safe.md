---
title: ต้องการทําเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281190"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>ต้องการทําเครื่องหมายโดเมนหรือผู้ส่งอีเมลที่ปลอดภัยหรือไม่

- **ไม่แนะนําให้ใช้รายชื่อผู้ส่งที่ปลอดภัย**เนื่องจากเปิดองค์กรของคุณเป็นสแปม ฟิช และการปลอมแปลง
- อย่างไรก็ตาม หากมีความต้องการทางธุรกิจ**เราขอแนะนําให้ใช้****[กฎขั้นตอนจดหมาย](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** สําหรับสิ่งนี้ คําแนะนําของเราทําให้การตรวจสอบสิทธิ์ผู้ส่ง (ตรวจสอบความถูกต้องของผู้ส่งไม่ได้ถูกปลอมแปลง) **หมายเหตุ**: เราไม่แนะนําให้จัดการค่าบวกที่ผิดพลาดโดยใช้รายชื่อผู้ส่งที่ปลอดภัย เนื่องจากข้อยกเว้นในการกรองสแปมสามารถเปิดองค์กรของคุณเพื่อการโจมตีด้านความปลอดภัยได้ ถ้าผู้ใช้ของคุณได้รับข้อความที่ถูกทําเครื่องหมายว่าเป็นอีเมลขยะหรืออีเมลขยะอย่างไม่ถูกต้อง**[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**
- ผู้ส่งที่ปลอดภัยใน Outlook รายชื่อผู้ส่งที่ได้รับอนุญาต หรือรายการที่อนุญาตในนโยบายป้องกันสแปม**ควรหลีกเลี่ยง**เนื่องจากผู้ส่งจะข้ามสแปม การปลอมแปลง และการป้องกันฟิชเชอร์ทั้งหมด และการตรวจสอบสิทธิ์ของผู้ส่ง (SPF, DKIM, DMARC) วิธีนี้จะใช้ได้ดีที่สุดสําหรับการทดสอบชั่วคราวเท่านั้น
