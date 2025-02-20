---
title: ตัวอย่าง Microsoft Defender Office 365นโยบายการป้องกันฟิชชิ่ง
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035025"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>ตัวอย่าง Microsoft Defender Office 365นโยบายการป้องกันฟิชชิ่ง

การตั้งค่าเหล่านี้จะเปิดใช้งานนโยบายที่เรียกว่า *โดเมนและ CEO* นโยบายนี้จะให้ทั้งการป้องกันผู้ใช้และโดเมนจากการเลียนแบบ จากนั้นจะปรับใช้นโยบายกับอีเมลทั้งหมดที่ได้รับโดยผู้ใช้ภายในโดเมน ก่อนอื่น ให้เพิ่มข้อมูลต่อไปนี้เพื่อสร้างนโยบาย

- **ชื่อ**: โดเมนและประธาน **เจ้าหน้าที่** บริหาร อธิบาย : ตรวจสอบให้แน่ใจว่า CEO และโดเมนของคุณจะไม่ถูกเลียนแบบ
  **ใช้กับ**: **เลือก โดเมนผู้รับ** คือ **ภายใต้ ตัวเลือก** เหล่านี้ **ให้เลือก** เลือก แล้วเลือกโดเมน เลือก **+** เพิ่ม เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากชื่อของโดเมนในรายการ (ตัวอย่างเช่น contoso.com )**แล้วเลือก** เพิ่ม เลือกเสร็จสิ้น
- หลังจากสร้างนโยบายแล้ว คุณสามารถปรับนโยบายให้ดีขึ้นได้โดยใช้ตัวเลือกต่อไปนี้
  - **เพิ่มผู้ใช้เพื่อป้องกัน:** ตัวอย่างนี้ให้เพิ่มที่อยู่อีเมลของ CEO อย่างน้อย
  - **เพิ่มโดเมนเพื่อป้องกัน**: เพิ่มโดเมนขององค์กรที่มีสํานักงาน CEO
  - **เลือก การ** แอคชัน **:** ถ้าอีเมลถูกส่งโดยผู้ใช้ที่เลียนแบบ ให้เลือก เปลี่ยนเส้นทางข้อความไปยังที่อยู่อีเมลอื่น แล้วใส่ที่อยู่อีเมลของผู้ดูแลระบบความปลอดภัย (ตัวอย่างเช่น *securityadmin@contoso.com*) For **ถ้าอีเมลถูกส่งโดยโดเมนที่เลียนแบบ** ให้เลือก **กักกัน** ข้อความ
  - **ข่าวกรอง** กล่องจดหมาย: ตามค่าเริ่มต้น ตัวเลือกนี้จะถูกเลือกเมื่อคุณสร้างนโยบายการป้องกันฟิชชิ่งใหม่ ปล่อยให้การตั้งค่า **นี้ เปิด** เพื่อผลลัพธ์ที่ดีที่สุด
  - **เพิ่มผู้ส่งและโดเมนที่เชื่อถือได้:** For this example, don't define any overrides.
- เมื่อคุณตรวจสอบการตั้งค่าของคุณแล้ว ให้เลือก **สร้างนโยบาย** นี้ **หรือ** บันทึก ตามความเหมาะสม

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู นโยบายการป้องกันฟิชชิ่งใน Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235)
