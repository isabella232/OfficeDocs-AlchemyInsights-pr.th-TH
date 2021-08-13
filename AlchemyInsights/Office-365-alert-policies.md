---
title: 1385-Office-365-alert-policies
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
ms.openlocfilehash: 7bb5ec0efb7e29dc6a133d62491c7674c5a851a4fa422c647035aeaa0dbcd8d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918378"
---
# <a name="alert-policies"></a>นโยบายการแจ้งเตือน

ศูนย์Microsoft 365การรักษาความปลอดภัยของ & Compliance มีนโยบายการแจ้งเตือนเริ่มต้นที่[](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)ทริกเกอร์การแจ้งเตือนให้กับองค์กรที่มีการสมัครใช้งาน Office 365 Enterprise หรือ Office 365 Government E1/G1, E3/G3 หรือ E5/G5 ดังนั้น ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลที่ส่งโดย Office365Alerts@microsoft.com ด้วยบรรทัดหัวเรื่อง เช่น "การแจ้งเตือนความรุนแรงต่า: ชื่อของ *นโยบาย* การแจ้งเตือน " การแจ้งเตือนจะถูกส่งเมื่อทริกเกอร์การแจ้งเตือนกิจกรรมทั่วไป เช่น เมื่อผู้ใช้:

- สร้างกฎกล่องจดหมายเข้าที่ส่งต่ออีเมล
- กําหนดสิทธิ์ให้กับกล่องจดหมายของพวกเขา
- แชร์หรือลบไฟล์จํานวนมากในSharePointการแชร์ไฟล์
- สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา

เมื่อต้องการตรวจสอบและกระบงการบนการแจ้งเตือน:

1. ไปที่ ศูนย์ [การรักษา&การปฏิบัติตามนโยบาย](https://protection.office.com) และลงชื่อเข้าใช้
2. คลิก  >  **การแจ้งเตือน ดู** การแจ้งเตือน
3. คลิกการแจ้งเตือนเพื่อแสดงหน้าฟลายเอาท์ที่มีข้อมูลเกี่ยวกับการแจ้งเตือนนั้น

คุณสามารถเริ่มการแจ้งเตือนได้ เช่น การ [เอากฎกล่องจดหมายเข้าที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)ออก หรือคุณสามารถปิดการแจ้งเตือนได้ด้วยการคลิก **แก้ไข** บนหน้าการแจ้งเตือนที่เมนูปลิว

For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**สิ่ง** สําคัญ: การแจ้งเตือนทางอีเมลแจ้งให้ทราบจาก Microsoft จะไม่ขอให้คุณส่งสิ่งต่อไปนี้:

- ใส่รหัสผ่าน
- ตรวจสอบรายละเอียดความปลอดภัยของบัญชีของคุณ
- รับรองความถูกต้องตัวคุณเองใหม่

ถ้าคุณได้รับข้อความอีเมลเช่นนี้ ข้อความนั้นจะไม่ถูกส่งโดย Microsoft และควรเป็นข้อความฟิชชิ่ง หากเกิดเหตุการณ์เช่นนี้[โปรดรายงานไปยัง Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)