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
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827235"
---
# <a name="using-dlp-in-transport-rules"></a>การใช้ DLP ในกฎการส่งผ่าน

เมื่อต้องการรวมการป้องกันการสูญหายของข้อมูล (DLP) ลงในการส่งผ่านที่มีอยู่ ให้ใช้เงื่อนไข "**ถ้าข้อความมี... ข้อมูลที่ละเอียดอ่อน**" ในการตั้งค่ากฎการส่งผ่าน

**ดูรายละเอียดเพิ่มเติมที่:**

- ชนิดข้อมูลที่เป็นความลับ DLP ที่รวมในกฎการส่งผ่าน:[รวมกฎของข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)

คุณยังสามารถทดสอบกฎที่มีหรือไม่ทดสอบนโยบายโดยใช้ โหมดการทดสอบ บนกฎได้  คุณควรรอ 30 นาทีหลังจากสร้างกฎก่อนการทดสอบ

- ดู [ทดสอบกฎของลโฟลว์/การส่งผ่านจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**หมายเหตุ**: ถ้าคุณพยายามปรับใช้นโยบาย DLP ใหม่กับกฎการส่งผ่านใน EAC ให้ใช้ [นโยบาย DLP ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) แทน
