---
title: จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure Windowsเดสก์ท็อปเสมือน
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
- "9003956"
- "7013"
ms.openlocfilehash: 260a0b2b8d3f8fcc1fd6096373a8a8ecd90585adc5865ff1fb832870cb62102e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53912077"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a>จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure Windowsเดสก์ท็อปเสมือน

กลุ่มแอปเริ่มต้นที่สร้างไว้Windowsพูลโฮสต์เดสก์ท็อปเสมือนจะเผยแพร่เดสก์ท็อปแบบเต็มด้วย นอกจากนี้ การใช้พอร์ทัล Azure ยังช่วยให้คุณสร้างกลุ่มแอป RemoteApp อย่างน้อยหนึ่งกลุ่มให้กับกลุ่มโฮสต์ได้

กระบวนการปรับใช้จะ:

1. สร้างกลุ่มแอป RemoteApp
2. เพิ่มแอปที่เลือกลงในกลุ่มแอป
3. เผยแพร่ผู้ใช้แต่ละรายหรือกลุ่มผู้ใช้ไปยังกลุ่มแอป
4. ลงทะเบียนกลุ่มแอป ถ้าคุณเลือกที่จะเข้าร่วม
5. สร้างลิงก์ไปยังเทมเพลต Azure Resource Manager ตามการกําหนดค่าของคุณ ที่คุณสามารถดาวน์โหลดและบันทึกได้

เมื่อต้องการสร้างกลุ่ม RemoteApp Windowsเดสก์ท็อปเสมือน ให้ปฏิบัติตามคําแนะนํา[ใน จัดการกลุ่มแอปด้วยพอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2129550)
