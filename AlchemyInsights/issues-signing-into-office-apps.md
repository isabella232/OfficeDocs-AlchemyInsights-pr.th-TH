---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579884"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขโปรแกรมประยุกต์ Microsoft 365 "โมดูลแพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณทํางานไม่ถูกต้อง"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองทําดังต่อไปนี้

- ติดตั้งการปรับปรุงล่าสุดสําหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \ซอฟต์แวร์\Microsoft\Office\16.0\ทั่วไป\รหัสประจําตัว\)
- ลอง[กระบวนการกู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)เพื่อแก้ไขความล้มเหลวของโมดูลแพลตฟอร์มที่เชื่อถือได้ (TPM)
- ตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:  
    1. คลิกขวาที่ปุ่ม เริ่ม ของ Windows เลือก**เรียกใช้**พิมพ์**regedit**แล้วเลือก**ตกลง**
    2. เลือก**ใช่**เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ
    3. ในตัวแก้ไขรีจิสทรี ให้เพิ่มค่า DWORD ของ**EnableADAL**ด้วยการตั้งค่า**0**ภายใต้ HKEY_CURRENT_USER\ซอฟต์แวร์\Microsoft\Office\16.0\Common\Identity

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากการปรับปรุง Office 2016 สร้าง 16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)