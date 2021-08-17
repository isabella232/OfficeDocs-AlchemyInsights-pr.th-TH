---
title: การใช้ DLP ในกฎการส่งผ่าน
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
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084113"
---
# <a name="using-dlp-in-transport-rules"></a>การใช้ DLP ในกฎการส่งผ่าน

เมื่อต้องการรวมการป้องกันการสูญหายของข้อมูล (DLP) ลงในการส่งผ่านที่มีอยู่ ให้ใช้เงื่อนไข "**ถ้าข้อความมี... ข้อมูลที่ละเอียดอ่อน**" ในการตั้งค่ากฎการส่งผ่าน

**ดูรายละเอียดเพิ่มเติมที่:**

- ชนิดข้อมูลที่เป็นความลับ DLP ที่รวมในกฎการส่งผ่าน:[รวมกฎของข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)

คุณยังสามารถทดสอบกฎที่มีหรือไม่ทดสอบนโยบายโดยใช้ โหมดการทดสอบ บนกฎได้  คุณควรรอ 30 นาทีหลังจากสร้างกฎก่อนการทดสอบ

- ดู[ทดสอบกฎการFlow/การส่งผ่านจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**หมายเหตุ**: ถ้าคุณพยายามปรับใช้นโยบาย DLP ใหม่กับกฎการส่งผ่านใน EAC ให้ใช้ [นโยบาย DLP ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) แทน
