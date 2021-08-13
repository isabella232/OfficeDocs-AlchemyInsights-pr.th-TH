---
title: บันทึกรหัสผ่าน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960962"
---
# <a name="password-logs"></a>บันทึกรหัสผ่าน

**ฉันมีปัญหาในการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่**

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่ ให้ปฏิบัติตามขั้นตอนต่อไปนี้

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดูบันทึกการตรวจสอบ 

บทบาทต่อไปนี้เท่านั้นที่ได้รับอนุญาต:
 - ผู้ดูแลระบบส่วนกลาง
 - ผู้ดูแลระบบความปลอดภัย
 - โปรแกรมอ่านความปลอดภัย

**ฉันต้องการดูเหตุการณ์การตรวจสอบการตั้งค่ารหัสผ่านใหม่ทั้งหมดตั้งแต่ที่ฉันปรับใช้ครั้งแรก**

การรีเซ็ตรหัสผ่าน/เหตุการณ์การลงทะเบียนสูงสุด 120,000 รายการจะถูกจัดเก็บไว้ในรายงานของ 30 วันที่ผ่านมา ขีดจํากัดสูงสุดนี้ใช้กับ UI เมื่อดาวน์โหลด CSV มีเหตุการณ์ 1 ล้านเหตุการณ์พร้อมใช้งานผ่านทาง PowerShell
ดูข้อมูลเพิ่มเติมที่ลิงก์ด้านล่าง:

- [เหตุการณ์รีเซ็ตรหัสผ่านแบบบริการตนเองจากรายงาน Azure AD และ API เหตุการณ์](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**ฉันต้องการเข้าใจเพิ่มเติมเกี่ยวกับความสามารถในการรายงานการรีเซ็ตรหัสผ่าน**

ตรวจสอบผู้ที่ลงทะเบียนหรือรีเซ็ตรหัสผ่านด้วยบันทึกการตรวจสอบการรีเซ็ตรหัสผ่าน Azure AD ในพอร์ทัล Azure **ภายใต้ ผู้ใช้และ** กลุ่ม
ดูข้อมูลเพิ่มเติมที่ลิงก์ต่อไปนี้:

- [ภาพรวมของรายงานการตั้งค่ารหัสผ่านใหม่](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดูรายงานรีเซ็ตรหัสผ่านในพอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [เหตุการณ์รีเซ็ตรหัสผ่านแบบบริการตนเองจากรายงาน Azure AD และ API เหตุการณ์](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


