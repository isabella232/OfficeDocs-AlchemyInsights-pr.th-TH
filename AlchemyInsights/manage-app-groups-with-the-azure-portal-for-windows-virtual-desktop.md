---
title: จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure สำหรับเดสก์ท็อปเสมือนของ Windows
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
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722053"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a>จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure สำหรับเดสก์ท็อปเสมือนของ Windows

กลุ่มแอปเริ่มต้นที่สร้างขึ้นสำหรับพูลโปรแกรมโฮสต์เดสก์ท็อปเสมือนใหม่ของ Windows จะเผยแพร่เดสก์ท็อปแบบเต็ม นอกจากนี้การใช้พอร์ทัล Azure จะช่วยให้คุณสามารถสร้างกลุ่มแอป RemoteApp อย่างน้อยหนึ่งกลุ่มสำหรับพูลโปรแกรมโฮสต์

กระบวนการปรับใช้จะดำเนินการดังต่อไปนี้:

1. สร้างกลุ่มแอป RemoteApp
2. เพิ่มแอปที่เลือกของคุณลงในกลุ่มแอป
3. ประกาศผู้ใช้แต่ละรายหรือกลุ่มผู้ใช้ไปยังกลุ่มแอป
4. ลงทะเบียนกลุ่มแอปถ้าคุณเลือกที่จะทำเช่นนั้น
5. สร้างลิงก์ไปยังแม่แบบตัวจัดการทรัพยากร Azure ตามการกำหนดค่าของคุณซึ่งคุณสามารถดาวน์โหลดและบันทึกได้

เมื่อต้องการสร้างกลุ่ม RemoteApp สำหรับเดสก์ท็อปเสมือนของ Windows ให้ทำตามคำแนะนำใน[จัดการกลุ่มแอปได้ด้วยพอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2129550)
