---
title: นโยบายการแจ้งเตือน 1385-Office-365
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
ms.openlocfilehash: 1209e59668bbe69fe88408933ae11b357b8d4f1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687637"
---
# <a name="alert-policies"></a>นโยบายการแจ้งเตือน

ศูนย์การปฏิบัติตามกฎระเบียบ & Microsoft 365 มี[นโยบายการแจ้งเตือนเริ่มต้น](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)ที่ทริกเกอร์การแจ้งเตือนสําหรับองค์กรที่มี Office 365 Enterprise หรือ Office 365 รัฐบาลสหรัฐ E1/G1, E3/G3 หรือการสมัครใช้งาน E5/G5 ผู้ดูแลอาจได้รับการแจ้งเตือนทางอีเมลที่ส่งโดยOffice365Alerts@microsoft.comบรรทัดเรื่องเช่น "การแจ้งเตือนความรุนแรงต่ํา:*ชื่อของนโยบายการแจ้งเตือน*" การแจ้งเตือนจะถูกส่งเมื่อทริกเกอร์การแจ้งเตือนสําหรับกิจกรรมทั่วไป เช่น เมื่อผู้ใช้:

- สร้างกฎกล่องจดหมายที่ส่งต่ออีเมล
- กําหนดสิทธิ์กล่องจดหมายของพวกเขา
- ใช้ร่วมกัน หรือลบไฟล์จํานวนมากใน SharePoint แฟ้มที่ใช้ร่วมกัน
- สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา

วิธีตรวจสอบและดําเนินการกับการแจ้งเตือน:

1. ไปที่[ศูนย์การปฏิบัติตามนโยบาย &ความปลอดภัยและ](https://protection.office.com)ลงชื่อเข้าใช้
2.  > คลิก**Alerts****การแจ้งเตือน**
3. คลิกการแจ้งเตือนเพื่อแสดงหน้าลอยพร้อมข้อมูลเกี่ยวกับการแจ้งเตือน

คุณสามารถดําเนินการกับการแจ้งเตือน เช่น[การลบกฎของกล่องจดหมายที่น่าสงสัย](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account) หรือคุณสามารถปิดการแจ้งเตือนได้โดยคลิก**แก้ไข**ที่หน้าลอยแจ้งเตือน

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าคอนฟิกและการจัดการนโยบายการแจ้งเตือน ให้ดูที่[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/alert-policies)

**สิ่งสําคัญ**: การแจ้งเตือนทางอีเมลจาก Microsoft จะไม่ขอให้คุณทําสิ่งต่อไปนี้:

- ใส่รหัสผ่าน
- ตรวจสอบรายละเอียดความปลอดภัยของบัญชีของคุณ
- ตรวจสอบความถูกต้องด้วยตนเองอีกครั้ง

หากคุณได้รับข้อความอีเมลเช่นนี้ Microsoft ไม่ได้ส่งและควรถือว่าเป็นการหลอกลวงแบบฟิชชิ่ง หากเกิดเหตุการณ์นี้โปรด[รายงานไปยัง Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)