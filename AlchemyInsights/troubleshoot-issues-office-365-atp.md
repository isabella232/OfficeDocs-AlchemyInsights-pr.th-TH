---
title: แก้ไขปัญหากับ Office 365 ขั้นสูงคุกคามป้องกัน (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031120"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>แก้ไขปัญหาเกี่ยวกับ Office 365 ATP

- **ความล่าช้าในการแจ้งให้ทราบ ด้วยการส่งข้อความอีเมล**หรือไม่ ลองใช้ตัวเลือกการจัดส่งแบบไดนามิกสำหรับนโยบาย ATP เซฟสิ่งที่แนบมาของคุณ ซึ่งจะช่วยหลีกเลี่ยงความล่าช้าที่ส่งข้อความอีเมล โดยผู้รับจากแฟ้มที่เป็นอันตราย
- **คุณต้องการทำงานผิดพลาด false รายงานหรือ false ค่าลบ**หรือไม่ ใช้การเชื่อมโยงนี้เพื่อส่งแฟ้มของคุณสำหรับการวิเคราะห์:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **คุณทราบว่า คุณสามารถเปิดใช้งานการป้องกันเชื่อมโยงเซฟ ATP สำหรับอีเมลที่ส่งระหว่างผู้คนในองค์กรของคุณ**ได้อย่างไร ทำตามขั้นตอนเหล่านี้:
    1. ไปที่https://protection.office.comและเข้าสู่ระบบ
    2. **จัดการความเสี่ยง**ไป > **นโยบาย** > **การเชื่อมโยงที่ปลอดภัย**
    3. ภายใต้**นโยบายที่นำไปใช้กับผู้รับที่ระบุ**แก้ไข (หรือเพิ่ม) นโยบาย
    4. เลือกการ**เชื่อมโยงเซฟนำไปใช้กับข้อความที่ส่งภายในองค์กร**
    5. บันทึกนโยบายของคุณ และอนุญาตให้ประมาณ 30 นาทีสำหรับการเปลี่ยนแปลงการทำงานของพวกเขารวด datacenter ของคุณ
- เมื่อต้องการขอความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ดู[การป้องกันภัยคุกคามขั้นสูงของ Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)