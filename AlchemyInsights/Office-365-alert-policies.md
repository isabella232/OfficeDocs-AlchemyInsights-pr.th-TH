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
ms.openlocfilehash: f5109445530ec4cc4988fb9c5d37145c45794ced6920607ce6df85c6497c25ec
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891698"
---
# <a name="alert-policies"></a>นโยบายการแจ้งเตือน

Microsoft 365[การแจ้งเตือนเริ่มต้นที่](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)ทริกเกอร์การแจ้งเตือนให้กับองค์กรที่มีการสมัครใช้งาน Microsoft 365 Enterprise หรือ Microsoft 365 Government E1/G1, E3/G3 หรือ E5/G5 ดังนั้น ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลที่ส่งโดย Office365Alerts@microsoft.com ด้วยบรรทัดหัวเรื่อง เช่น "การแจ้งเตือนความรุนแรงต่า: ชื่อของ *นโยบาย* การแจ้งเตือน " การแจ้งเตือนจะถูกส่งเมื่อทริกเกอร์การแจ้งเตือนกิจกรรมทั่วไป เช่น เมื่อผู้ใช้:

- สร้างกฎกล่องจดหมายเข้าที่ส่งต่ออีเมล
- กําหนดสิทธิ์ให้กับกล่องจดหมายของพวกเขา
- แชร์หรือลบไฟล์จํานวนมากในSharePointการแชร์ไฟล์
- สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา

เมื่อต้องการตรวจสอบและกระบงการบนการแจ้งเตือน:

1. ให้เลือกปฏิบัติตามขั้นตอนใดขั้นตอนหนึ่งต่อไปนี้
   - ศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 <https://compliance.microsoft.com> การแจ้งเตือน **ที่ ไปที่** การแจ้งเตือน หรือเมื่อต้องการไปที่ **หน้า** การแจ้งเตือน <https://compliance.microsoft.com/compliancealerts> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderการแจ้งเตือน <https://security.microsoft.com> ที่ **ให้ไปที่ เหตุการณ์&** \> **การแจ้งเตือน** หรือเมื่อต้องการไปที่ **หน้า** การแจ้งเตือน <https://security.microsoft.com/alerts> โดยตรง ให้ใช้
2. คลิกการแจ้งเตือนเพื่อแสดงหน้าฟลายเอาท์ที่มีข้อมูลเกี่ยวกับการแจ้งเตือนนั้น

คุณสามารถเริ่มการแจ้งเตือนได้ เช่น การ [เอากฎกล่องจดหมายเข้าที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)ออก หรือคุณสามารถปิดการแจ้งเตือนได้ด้วยการคลิก **แก้ไข** บนหน้าการแจ้งเตือนที่เมนูปลิว

For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**สิ่ง** สําคัญ: การแจ้งเตือนทางอีเมลแจ้งให้ทราบจาก Microsoft จะไม่ขอให้คุณส่งสิ่งต่อไปนี้:

- ใส่รหัสผ่าน
- ตรวจสอบรายละเอียดความปลอดภัยของบัญชีของคุณ
- รับรองความถูกต้องตัวคุณเองใหม่

ถ้าคุณได้รับข้อความอีเมลที่มีชนิดการร้องขอเหล่านี้ ข้อความนั้นจะไม่ถูกส่งโดย Microsoft และควรถือว่าเป็นการฟิชชิ่ง ถ้าคุณได้รับข้อความที่มีชนิดการร้องขอเหล่านี้[ให้รายงานข้อความไปยัง Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)
