---
title: แก้ไขปัญหาเกี่ยวกับการป้องกันภัยคุกคามขั้นสูงของ Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511131"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>แก้ไขปัญหาเกี่ยวกับ Atp ของ Office 365

- **แจ้งความล่าช้ากับการส่งข้อความอีเมล์**? ลองใช้ตัวเลือกการจัดส่งแบบไดนามิกสําหรับนโยบายสิ่งที่แนบมาที่ปลอดภัย ATP ของคุณ การทําเช่นนี้จะหลีกเลี่ยงความล่าช้าในการจัดส่งข้อความอีเมลในขณะที่ปกป้องผู้รับจากแฟ้มที่เป็นอันตราย
- **คุณต้องการรายงานผลบวกเท็จหรือเชิงลบเท็จ**หรือไม่ ใช้ลิงก์นี้เพื่อส่งไฟล์ของคุณสําหรับการวิเคราะห์:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันการเชื่อมโยงที่ปลอดภัยของ ATP สําหรับอีเมลที่ส่งระหว่างคนในองค์กรของคุณ**? ทําตามขั้นตอนต่อไปนี้
    1. ไปที่ https://protection.office.com และลงชื่อเข้าใช้
    2. ไปที่นโยบาย**การจัดการภัยคุกคาม**  >  **Policy**  >  **การเชื่อมโยงที่ปลอดภัย**
    3. ภายใต้**นโยบายที่ใช้กับผู้รับที่ระบุ**ให้แก้ไข (หรือเพิ่ม) นโยบาย
    4. เลือก**ใช้การเชื่อมโยงที่ปลอดภัยกับข้อความที่ส่งภายในองค์กร**
    5. บันทึกนโยบายของคุณ และอนุญาตให้ประมาณ 30 นาทีเพื่อให้การเปลี่ยนแปลงของคุณทํางานผ่านศูนย์ข้อมูลของคุณ
- เมื่อต้องการรับความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ให้ดูที่[การป้องกันภัยคุกคามขั้นสูงของ Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)