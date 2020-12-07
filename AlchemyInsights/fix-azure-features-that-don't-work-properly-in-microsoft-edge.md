---
title: สิ่งที่ต้องทำถ้าฟีเจอร์ Azure ทำงานไม่ถูกต้องใน Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583780"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>สิ่งที่ต้องทำถ้าฟีเจอร์ Azure ทำงานไม่ถูกต้องใน Microsoft Edge

Microsoft Edge ได้ [ทราบปัญหา](https://go.microsoft.com/fwlink/?linkid=2140608) ที่เกี่ยวข้องกับโซนความปลอดภัยและอาจส่งผลต่อวิธีการเข้าสู่ระบบของผู้ใช้ Azure ในศูนย์การจัดการ Windows ถ้าคุณกำลังมีปัญหาในการใช้ฟีเจอร์ Azure กับ Microsoft Edge ให้ลองทำตามขั้นตอนต่อไปนี้:

1. ในเมนู **เริ่ม** ให้ค้นหา **ตัวเลือกอินเทอร์เน็ต** แล้วเลือก
2. ในกล่องโต้ตอบ **คุณสมบัติของอินเทอร์เน็ต** ให้ไปที่แท็บ **ความปลอดภัย**
3. เลือกโซน **ไซต์ที่เชื่อถือ** ได้แล้วเลือกปุ่ม **ไซต์**
4. ในกล่องโต้ตอบ **ไซต์ที่เชื่อถือได้** ให้เพิ่ม URL ของเกตเวย์ของคุณเช่นเดียวกับ [https://login.microsoftonline.com](https://login.microsoftonline.com) และ [https://login.live.com](https://login.live.com) จากนั้นเลือก **ปิด**
5. ในกล่องโต้ตอบ **คุณสมบัติของอินเทอร์เน็ต** ให้ไปที่แท็บ **ความเป็นส่วนตัว**
6. ในส่วนตัว **บล็อก** ป็อปอัพให้เลือก **การตั้งค่า** ในกล่องโต้ตอบที่เปิดขึ้นให้เพิ่ม URL ของเกตเวย์ของคุณรวมถึง [https://login.microsoftonline.com](https://login.microsoftonline.com) และ [https://login.live.com](https://login.live.com) จากนั้นเลือก **ปิด**
