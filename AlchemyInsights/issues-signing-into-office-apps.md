---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833034"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขข้อความ "โมดูลแพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณมีฟังก์ชันการฟังก์ชันไม่ถูกต้อง" ของแอป Microsoft 365

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองวิธีต่อไปนี้:

- ติดตั้งการอัปเดตล่าสุดของ[Windows](https://support.microsoft.com/help/4027667/windows-10-update) [และ Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)
- ลองกระบวนการ [กู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)
- ตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:  
    1. คลิกขวาที่ปุ่ม เริ่ม ของ Windows **เลือก** เรียกใช้ **พิมพ์ regedit****แล้วเลือก** ตกลง
    2. เลือก **ใช่** เพื่ออนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ
    3. ใน Registry Editor ให้เพิ่มค่า DWORD ของ **EnableADAL** ด้วยการตั้งค่า **0** ภายใต้ HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity

For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).