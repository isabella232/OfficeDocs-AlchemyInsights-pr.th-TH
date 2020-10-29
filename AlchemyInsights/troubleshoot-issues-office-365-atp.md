---
title: แก้ไขปัญหาเกี่ยวกับ Microsoft Defender สำหรับ Office ๓๖๕ (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801426"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>การแก้ไขปัญหาเกี่ยวกับ Office ๓๖๕ ATP

- การ **แจ้งเตือนล่าช้าด้วยการส่งข้อความอีเมล** ลองใช้ตัวเลือกการนำส่งแบบไดนามิกสำหรับนโยบายสิ่งที่แนบมาของ ATP Safe ของคุณ วิธีนี้จะหลีกเลี่ยงความล่าช้าในการนำส่งข้อความอีเมลในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย
- **คุณต้องการรายงาน false บวกหรือ** ค่าลบ false หรือไม่ ใช้ลิงก์นี้เพื่อส่งไฟล์ของคุณสำหรับการวิเคราะห์: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันการเชื่อมโยงที่ปลอดภัยของ ATP สำหรับอีเมลที่ส่งระหว่างบุคคลในองค์กรของคุณ** ให้ทำตามขั้นตอนต่อไปนี้:
    1. ไปที่ https://protection.office.com แล้วลงชื่อเข้าใช้
    2. ไปที่ **Threat management**  >  **Policy**  >  **ลิงก์ความปลอดภัย** ของนโยบายการจัดการภัยคุกคาม
    3. ภายใต้ **นโยบายที่นำไปใช้กับผู้รับที่ระบุ** แก้ไข (หรือเพิ่ม) นโยบาย
    4. เลือก **นำลิงก์ที่ปลอดภัยไปใช้กับข้อความที่ส่งภายในองค์กร**
    5. บันทึกนโยบายของคุณและอนุญาตให้ใช้เวลาประมาณ30นาทีเพื่อให้การเปลี่ยนแปลงของคุณทำงานผ่านทางศูนย์ข้อมูลของคุณ
- เมื่อต้องการรับความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ให้ดูที่[Microsoft Defender สำหรับ Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)