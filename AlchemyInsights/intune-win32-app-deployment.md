---
title: การปรับใช้แอป Intun1 Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925904"
---
# <a name="intune-win32-app-deployment"></a>การปรับใช้แอป Intun1 Win32

Microsoft Intuneอนุญาตแอปพลิเคชัน Win32 รวมถึง แต่ไม่จํากัดเฉพาะ MSI .EXEของ Windows เพื่อใช้งานWindows 10อื่นได้ กลไกการปรับใช้ที่ใช้ต้องการให้ส่วนขยายการจัดการ Intun1 (IME) อยู่บนอุปกรณ์เป้าหมาย IME จะถูกติดตั้งโดยอัตโนมัติเป็นผลจากการ targeting a powershell script or win32 application deployment to a user / device.

นอกจากนี้ยังมีชุดเงื่อนไขก่อนที่ต้องพบเพื่อปรับใช้แอป Win32 ซึ่งรวมถึง:

- แพลตฟอร์มที่รองรับ: Windows 10เวอร์ชัน 1607 หรือใหม่กว่า (เวอร์ชัน Enterprise, Pro และ Education)
- สถาปัตยกรรมที่รองรับ: x86 และ x64
- การจัดการอุปกรณ์: AAD เข้าร่วมและลงทะเบียนโดยอัตโนมัติ (รวมถึงโดเมนแบบไฮบริดที่เข้าร่วมและนโยบายกลุ่มโดยอัตโนมัติ)
- รูปแบบแอปพลิเคชันแพคเกจ: **intun1win**  file prepared by [the Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- ข้อจํากัด:
    - ขนาดสูงสุด: 8 GB
    - สถาปัตยกรรมที่ไม่ได้รับการสนับสนุน: ARMs

ตรวจทานเอกสาร "[เพิ่ม มอบหมาย และตรวจสอบแอป Win32 Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" เพื่อดูข้อมูลเกี่ยวกับขั้นตอนเหล่านั้น

รายละเอียดเกี่ยวกับการแก้ไขปัญหาการปรับใช้แอปพลิเคชันWindowsรวมถึงแอป Win32 สามารถตรวจสอบได้ในเอกสารต่อไปนี้

- [แก้ไขปัญหาการติดตั้งแอป](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [แก้ไขปัญหาแอป Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)