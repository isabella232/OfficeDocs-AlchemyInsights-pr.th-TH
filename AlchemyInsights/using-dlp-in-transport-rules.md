---
title: การใช้ DLP ในกฎการขนส่ง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915297"
---
# <a name="using-dlp-in-transport-rules"></a>การใช้ DLP ในกฎการขนส่ง

เมื่อต้องการรวมการป้องกันข้อมูลสูญหาย (DLP) ลงในการขนส่งที่มีอยู่ ให้ใช้เงื่อนไข "**ถ้าข้อความมี... ข้อมูลที่สําคัญ**" ในการตั้งค่ากฎการขนส่ง

**สําหรับรายละเอียดเพิ่มเติม โปรดดูที่:**

- ชนิดข้อมูลที่ละเอียดอ่อน DLP แบบรวมในกฎการขนส่ง:[รวมกฎข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)

นอกจากนี้คุณยังสามารถทดสอบกฎที่มีหรือไม่มีการทดสอบนโยบายโดยใช้โหมดทดสอบในกฎ  คุณควรรอ 30 นาทีหลังจากสร้างกฎก่อนที่จะทดสอบมัน.

- ดู[ทดสอบกฎลําดับ/การขนส่งจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**หมายเหตุ**: ถ้าคุณกําลังพยายามใช้นโยบาย DLP ใหม่ กับกฎการขนส่งใน EAC ใช้[นโยบาย DLP ในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)แทน
