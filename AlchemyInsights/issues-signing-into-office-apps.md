---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕
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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695198"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>การแก้ไขแอป Microsoft ๓๖๕ "โมดูลของ Platform ที่เชื่อถือได้ของคอมพิวเตอร์ของคุณไม่ทำงานอย่างถูกต้อง"

เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองทำดังต่อไปนี้:

- ติดตั้งการอัปเดตล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)
- ลอง [ใช้กระบวนการกู้คืนของผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของโมดูลของ PLATFORM (TPM) ที่เชื่อถือได้
- ตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:  
    1. คลิกขวาที่ปุ่มเริ่มของ Windows แล้วเลือก**เรียกใช้**พิมพ์**regedit**จากนั้นเลือก**ตกลง**
    2. เลือก **ใช่** เพื่ออนุญาตให้แก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ
    3. ใน Registry Editor ให้เพิ่มค่า DWORD ของ **EnableADAL** ที่มีการตั้งค่า **0** ภายใต้ HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office ๒๐๑๖รุ่น16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)