---
title: 1385-Office-365-การแจ้งเตือน-นโยบาย
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502446"
---
# <a name="alert-policies"></a>นโยบายการแจ้งเตือน

ศูนย์การปฏิบัติตามกฎระเบียบ& Microsoft 365 มี[นโยบายการแจ้งเตือนเริ่มต้น](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)ที่ทริกเกอร์การแจ้งเตือนสําหรับองค์กรที่มี Office 365 องค์กรหรือ Office 365 รัฐบาลสหรัฐ E1/G1, E3/G3 หรือ E5/G5 การสมัครใช้งาน ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลที่ส่งโดยOffice365Alerts@microsoft.comกับบรรทัดเรื่องเช่น "การแจ้งเตือนความรุนแรงต่ํา:*ชื่อของนโยบายการแจ้งเตือน*" การแจ้งเตือนจะถูกส่งเมื่อมีการทริกเกอร์การแจ้งเตือนสําหรับกิจกรรมทั่วไป เช่น เมื่อผู้ใช้:

- สร้างกฎของกล่องขาเข้าที่ส่งต่ออีเมล
- กําหนดสิทธิ์ในกล่องจดหมาย
- แชร์หรือลบแฟ้มจํานวนมากในการแชร์ไฟล์ SharePoint
- สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา

วิธีตรวจสอบและดําเนินการกับการแจ้งเตือน:

1. ไปที่[ศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย](https://protection.office.com)และลงชื่อเข้าใช้
2. คลิก**Alerts**  >  **การแจ้งเตือนมุมมอง**การแจ้งเตือน
3. คลิกการแจ้งเตือนเพื่อแสดงหน้าลอยพร้อมข้อมูลเกี่ยวกับการแจ้งเตือน

คุณสามารถดําเนินการกับการแจ้งเตือน เช่น[การลบกฎกล่องจดหมายที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) หรือคุณสามารถปิดการแจ้งเตือนได้โดยคลิก**แก้ไข**ในหน้าการแจ้งเตือน

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าคอนฟิกและการจัดการนโยบายการแจ้งเตือน ให้ดูที่[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**สําคัญ**: การแจ้งเตือนอีเมลแจ้งเตือนจาก Microsoft จะไม่ขอให้คุณทําสิ่งต่อไปนี้:

- ใส่รหัสผ่าน
- ยืนยันรายละเอียดความปลอดภัยของบัญชีของคุณ
- ตรวจสอบตัวตนใหม่ด้วยตัวคุณเอง

หากคุณได้รับข้อความอีเมลเช่นนี้ Microsoft จะไม่ถูกส่งมา และควรได้รับการพิจารณาว่าเป็นฟิชชิ่ง หากเกิดเหตุการณ์ดังกล่าวโปรด[รายงานไปยัง Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)