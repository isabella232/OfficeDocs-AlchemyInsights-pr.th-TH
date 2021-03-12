---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709125"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขแอป Microsoft 365 ข้อความ "แพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณไม่ฟังก์ชันอย่างถูกต้อง"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ลองต่อไปนี้:

- ติดตั้งการอัปเดตล่าสุดของ[Windows](https://support.microsoft.com/help/4027667/windows-10-update) [และ Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)
- ลองกระบวนการ [กู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)
- ตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:  
    1. คลิกขวาที่ปุ่ม เริ่ม ของ Windows เลือก **เรียกใช้** พิมพ์ **regedit****แล้วเลือก** ตกลง
    2. เลือกใช่ เพื่ออนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ
    3. ใน Registry Editor ให้เพิ่มค่า DWORD ของ **EnableADAL** ที่มีการตั้งค่า **เป็น 0** ภายใต้ HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity

For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).