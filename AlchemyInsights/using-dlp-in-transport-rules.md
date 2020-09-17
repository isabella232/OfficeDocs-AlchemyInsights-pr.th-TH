---
title: การใช้ DLP ในกฎการขนส่ง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773182"
---
# <a name="using-dlp-in-transport-rules"></a>การใช้ DLP ในกฎการขนส่ง

เมื่อต้องการรวมการป้องกันการสูญหายของข้อมูล (DLP) ลงในการขนส่งที่มีอยู่ให้ใช้เงื่อนไข "**ถ้าข้อความมี ... ข้อมูลที่ละเอียดอ่อน**"ในการตั้งค่ากฎการขนส่ง

**สำหรับรายละเอียดเพิ่มเติมให้ดูที่:**

- ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ที่รวมอยู่ในกฎการขนส่ง:[รวมกฎข้อมูลที่สำคัญ](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)

นอกจากนี้คุณยังสามารถทดสอบกฎที่มีหรือไม่มีการทดสอบนโยบายโดยใช้โหมดทดสอบบนกฎได้  คุณควรรอ30นาทีหลังจากสร้างกฎก่อนที่จะทดสอบ

- ดู [ทดสอบการรับส่งจดหมาย/กฎการขนส่ง](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**หมายเหตุ**: ถ้าคุณกำลังพยายามดำเนินการนโยบาย DLP ใหม่กับกฎการส่งผ่านใน EAC ให้ใช้ [นโยบาย dlp ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) แทน
