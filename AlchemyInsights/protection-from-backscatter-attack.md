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
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911249"
---
# <a name="protection-from-backscatter-attack"></a>การป้องกันจากการโจมตีจากระบบตีกลับ

ระบบตีกลับเป็นรายงานแจ้งการไม่สามารถส่งได้ (หรือที่เรียกว่า NDR หรือข้อความแจ้งการตีกลับ) ที่คุณได้รับจากข้อความที่คุณยังไม่ได้ส่ง สแปมเมอร์ปลอมแปลง (ปลอมแปลง) ที่อยู่ **จาก:** ของข้อความของพวกเขา และพวกเขามักจะใช้ที่อยู่อีเมลจริงเพื่อให้เกิดความน่าเชื่อถือกับข้อความของพวกเขา ดังนั้น เมื่อผู้ส่งสแปมส่งข้อความไปยังผู้รับที่ไม่มีอยู่อย่างหลีกเลี่ยงไม่ได้ เซิร์ฟเวอร์อีเมลปลายทางจะหลอกลวงให้ส่งกลับข้อความที่ไม่สามารถส่งได้ใน NDR ไปยังผู้ส่งที่ปลอมแปลงในที่อยู่ **จาก:**

ข้อมูลเพิ่มเติมสามารถพบได้ใน[ระบบการย้อนกลับใน EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**การเปิดใช้งานการป้องกันระบบรับและป้องกันระบบรับและกระท้บ**

เมื่อต้องการเปิดใช้งานการป้องกันระบบป้องกันระบบป้องกันแบบ Backscatter ให้ปฏิบัติตามเส้นทางด้านล่าง

**protection.office.com > Threat Management > > Antispam > เลือกนโยบายตัวกรองสแปมและ แก้ไขนโยบาย > คุณสมบัติสแปม > การตรวจหาและตีกลับ > NDR > ตั้งค่าเป็น "เปิด"**

ถ้าคุณเชื่อว่าบัญชีถูกละเมิด ดูรายการต่อไปนี้:

- [การตอบสนองต่อบัญชีอีเมลที่ถูกละเมิด](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [การเอาผู้ใช้ที่ถูกบล็อกออกจากพอร์ทัลผู้ใช้ที่ถูกOffice 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



