---
title: การป้องกันจากการโจมตีจากระบบตีกลับ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037181"
---
# <a name="protection-from-backscatter-attack"></a>การป้องกันจากการโจมตีจากระบบตีกลับ

ระบบตีกลับเป็นรายงานแจ้งการไม่สามารถส่งได้ (หรือที่เรียกว่า NRS หรือข้อความแจ้งการตีกลับ) ที่คุณได้รับจากข้อความที่คุณยังไม่ได้ส่ง สแปมเมอร์ปลอมแปลง (ปลอมแปลง) ที่อยู่ **จาก:** ของข้อความของพวกเขา และมักใช้ที่อยู่อีเมลจริงเพื่อให้ข้อความเหล่านั้นมีความน่าเชื่อถือ ดังนั้น เมื่อผู้ส่งสแปมส่งข้อความไปยังผู้รับที่ไม่มีอยู่อย่างหลีกเลี่ยงไม่ได้ เซิร์ฟเวอร์อีเมลปลายทางอาจหลอกลวงให้ส่งกลับข้อความที่ไม่สามารถส่งได้ใน NDR ไปยังผู้ส่งที่ปลอมแปลงในที่อยู่ **จาก:**

ข้อมูลเพิ่มเติมสามารถพบได้ใน[ระบบ Backscatter ใน EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**การเปิดใช้งานการป้องกันระบบป้องกันระบบป้องกันระบบกระทกหลัง**

เมื่อต้องการเปิดใช้งานการป้องกันระบบกลับ ให้ปฏิบัติตามเส้นทางด้านล่าง

**protection.office.com > Threat Management > > Antispam > เลือกนโยบายตัวกรองสแปมและแก้ไขนโยบาย > คุณสมบัติสแปม > > การตรวจหาและตีกลับ NDR > ตั้งเป็น "เปิด"**

ถ้าคุณเชื่อว่าบัญชีถูกละเมิด ให้ดูรายการต่อไปนี้:

- [การตอบสนองต่อบัญชีอีเมลที่ถูกละเมิด](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [การเอาผู้ใช้ที่ถูกบล็อกออกจากพอร์ทัลผู้ใช้ที่ถูกบล็อกใน Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



