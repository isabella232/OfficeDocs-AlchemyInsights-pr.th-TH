---
title: ๑๓๘๕-Office-๓๖๕-การแจ้งเตือน-นโยบาย
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664045"
---
# <a name="alert-policies"></a>นโยบายการแจ้งเตือน

ศูนย์การรักษาความปลอดภัย & ของ Microsoft ๓๖๕มี [นโยบายการแจ้งเตือนเริ่มต้น](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) ที่ทริกเกอร์การแจ้งเตือนสำหรับองค์กรที่มี Office ๓๖๕ Enterprise หรือ Office ๓๖๕สหรัฐอเมริการัฐ E1/G1, E3/G3 หรือการสมัครใช้งานแบบ E5/G5/G5 ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลการแจ้งเตือนที่ส่งโดย Office365Alerts@microsoft.com กับบรรทัดชื่อเรื่องเช่น "การแจ้งเตือนความรุนแรงต่ำ: *ชื่อของนโยบายการแจ้งเตือน*" การแจ้งเตือนจะถูกส่งเมื่อข้อความแจ้งเตือนถูกทริกเกอร์สำหรับกิจกรรมทั่วไปเช่นเมื่อผู้ใช้:

- สร้างกฎกล่องจดหมายเข้าที่ส่งต่ออีเมล
- กำหนดสิทธิ์กล่องจดหมายของพวกเขา
- แชร์หรือลบไฟล์จำนวนมากในการแชร์ไฟล์ SharePoint
- สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา

เมื่อต้องการตรวจสอบและดำเนินการกับการแจ้งเตือน:

1. ไปที่ [ศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย](https://protection.office.com) และลงชื่อเข้าใช้
2. คลิ**กการแจ้งเตือน**  >  **มุมมอง**การแจ้งเตือน
3. คลิกที่การแจ้งเตือนเพื่อแสดงหน้าลอยที่มีข้อมูลเกี่ยวกับการแจ้งเตือน

คุณสามารถดำเนินการกับการแจ้งเตือนเช่นการ [เอากฎกล่องจดหมายเข้าที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)ออก หรือคุณก็สามารถปิดการแจ้งเตือนได้โดยการคลิก **แก้ไข** บนหน้าเมนูลอยตัวของการแจ้งเตือน

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดค่าและการจัดการนโยบายการแจ้งเตือนให้ดู[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**สิ่งสำคัญ**: การแจ้งเตือนทางอีเมลที่แจ้งเตือนจาก Microsoft จะไม่ขอให้คุณทำดังต่อไปนี้:

- ใส่รหัสผ่าน
- ตรวจสอบรายละเอียดความปลอดภัยของบัญชีผู้ใช้ของคุณ
- การรับรองความถูกต้องอีกครั้งด้วยตัวคุณเอง

ถ้าคุณได้รับข้อความอีเมลที่มีข้อความนี้ไม่ได้ถูกส่งโดยไมโครซอฟท์และควรถือว่าเป็นการหลอกลวงฟิชชิ่ง ถ้าเกิดเหตุการณ์ดังกล่าวโปรด[รายงานข้อมูลนั้นไปยังไมโครซอฟท์](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)