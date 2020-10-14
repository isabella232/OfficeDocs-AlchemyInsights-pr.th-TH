---
title: การปรับใช้แอป Intune Win32
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
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461995"
---
# <a name="intune-win32-app-deployment"></a>การปรับใช้แอป Intune Win32

Microsoft Intune ช่วยให้แอปพลิเคชัน Win32 รวมถึงแต่ไม่จำกัดเฉพาะ MSI และ EXE ของคุณสามารถปรับใช้กับอุปกรณ์ Windows 10 ได้ กลไกการปรับใช้ที่ใช้จำเป็นต้องมีส่วนขยายการจัดการ Intune (IME) ที่จะนำเสนอบนอุปกรณ์เป้าหมาย IME จะได้รับการติดตั้งโดยอัตโนมัติเป็นผลลัพธ์ของการกำหนดเป้าหมายสคริปต์ powershell หรือการปรับใช้แอปพลิเคชัน win32 กับผู้ใช้/อุปกรณ์

นอกจากนี้ยังมีชุดของ requisites ที่ต้องตรงตามลำดับเพื่อปรับใช้แอปพลิเคชัน Win32 ซึ่งรวมถึง:

- แพลตฟอร์มที่ได้รับการสนับสนุน: Windows 10 เวอร์ชัน๑๖๐๗หรือเวอร์ชันที่ใหม่กว่า (Enterprise, Pro และการศึกษา)
- สถาปัตยกรรมที่ได้รับการสนับสนุน: x86 และ x64
- การจัดการอุปกรณ์: AAD เข้าร่วมและลงทะเบียนโดยอัตโนมัติ (รวมถึงการเข้าร่วมโดเมนแบบไฮบริดและการลงทะเบียนนโยบายกลุ่มโดยอัตโนมัติ)
- รูปแบบแพคเกจแอปพลิเคชัน: ไฟล์**intunewin**ที่เตรียมโดย[เครื่องมือการเตรียมเนื้อหาของ Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)
- ข้อจำกัด
    - ขนาดสูงสุด: 8GB
    - สถาปัตยกรรมที่ไม่ได้รับการสนับสนุน: แขน

ตรวจทานเอกสาร "[เพิ่มมอบหมายและตรวจสอบแอป Win32 ใน Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" สำหรับข้อมูลที่เกี่ยวข้องกับขั้นตอนเหล่านั้น

รายละเอียดเกี่ยวกับการแก้ไขปัญหาการปรับใช้แอปพลิเคชันบน Windows รวมถึงแอป Win32 ที่สามารถรีวิวได้ในเอกสารต่อไปนี้

- [แก้ไขปัญหาการติดตั้งแอป](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [การแก้ปัญหาแอป Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)