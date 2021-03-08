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
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527777"
---
# <a name="password-logs"></a>บันทึกรหัสผ่าน

**ฉันมีปัญหาในการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่**

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่ ให้ปฏิบัติตามขั้นตอนต่อไปนี้

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดูบันทึกการตรวจสอบ 

บทบาทต่อไปนี้ได้รับอนุญาตเท่านั้น:
 - ผู้ดูแลระบบส่วนกลาง
 - ผู้ดูแลระบบความปลอดภัย
 - โปรแกรมอ่านความปลอดภัย

**ฉันต้องการดูเหตุการณ์การตรวจสอบการตั้งค่ารหัสผ่านใหม่ทั้งหมดตั้งแต่ที่ฉันปรับใช้ครั้งแรก**

การรีเซ็ตหรือการลงทะเบียนรหัสผ่านสูงสุด 120,000 รายการจะถูกเก็บไว้ในรายงานของ 30 วันที่ผ่านมา ขีดจํากัดสูงสุดนี้ใช้กับ UI เมื่อดาวน์โหลด CSV มีเหตุการณ์ 1 ล้านเหตุการณ์ผ่าน PowerShell
ดูลิงก์ทางด้านล่างเพื่อดูข้อมูลเพิ่มเติม:

- [เหตุการณ์การรีเซ็ตรหัสผ่านด้วยตนเองจากรายงาน Azure AD และ API เหตุการณ์](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**ฉันต้องการเข้าใจเพิ่มเติมเกี่ยวกับความสามารถในการรายงานการรีเซ็ตรหัสผ่าน**

ตรวจสอบผู้ที่ลงทะเบียนหรือรีเซ็ตรหัสผ่านด้วยบันทึกการตรวจสอบการรีเซ็ตรหัสผ่าน Azure AD ในพอร์ทัล Azure **ภายใต้ผู้ใช้และ** กลุ่ม
ดูลิงก์ต่อไปนี้เพื่อดูข้อมูลเพิ่มเติม:

- [ภาพรวมรายงานการตั้งค่ารหัสผ่านใหม่](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดูรายงานรีเซ็ตรหัสผ่านในพอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [เหตุการณ์การรีเซ็ตรหัสผ่านด้วยตนเองจากรายงาน Azure AD และ API เหตุการณ์](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


