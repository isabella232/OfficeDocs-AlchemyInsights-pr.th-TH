---
title: ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938368"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>แก้ไขข้อความ "โมดูลแพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณทำงานได้อย่างถูกต้อง" โปรแกรมประยุกต์ Office

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ลองต่อไปนี้:

- ติดตั้งโปรแกรมปรับปรุงล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0 (แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)
- ลอง[กระบวนการกู้คืนข้อมูลของผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)เมื่อต้องการแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)
- EnableADAL ที่ตั้ง = 0 โดยใช้ขั้นตอนต่อไปนี้:  
    1. คลิกขวาปุ่มเริ่ม Windows เลือก**เรียกใช้**พิมพ์**regedit**จากนั้น เลือก**ตกลง**
    2. เลือก**ใช่**เพื่ออนุญาตให้ใช้ตัวแก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ
    3. ใน Registry Editor เพิ่มค่า DWORD ของ**EnableADAL**ด้วยการตั้งค่าที่**0**ภายใต้ HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity

สำหรับข้อมูลเพิ่มเติม ดู[ปัญหาการเชื่อมต่อในเครื่องหลังจากการปรับปรุง Office 2016 build 16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)