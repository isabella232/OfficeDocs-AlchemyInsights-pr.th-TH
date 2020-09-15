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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695306"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>หน้าจอการลงชื่อเข้าใช้เปล่าในแอป Microsoft ๓๖๕

เมื่อต้องการแก้ไขปัญหานี้ให้ลองทำดังต่อไปนี้:
- ติดตั้งการอัปเดตล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- ตั้งค่าตัวเลือก internet explorer ใหม่: ไปที่**เครื่องมือ**  >  **ตัวเลือก**  >  **Advanced**  >  **การตั้งค่า internet explorer**ขั้นสูงตั้งค่าใหม่ (โปรดทราบว่าคุณจะสูญเสียการตั้งค่าแบบกำหนดเอง) แล้วลองลงชื่อเข้าใช้ Office อีกครั้ง
- ปิดใช้งานแอปพลิเคชัน Windows Defender Guard (WDAG) หรือไฟร์วอลล์ที่คล้ายกันหรือโปรแกรมป้องกันไวรัส:
    1. ในแผงควบคุมให้ไปที่**โปรแกรม**แล้วเลือก**เปิดหรือปิดฟีเจอร์ของ Windows**
    2. ถ้าเปิดใช้งาน Guard ของแอปพลิเคชัน Windows Defender ให้ลองปิดใช้งาน<br/>
    **หมายเหตุ:** คุณอาจจำเป็นต้องเริ่มการทำงานของคอมพิวเตอร์ใหม่
- ตรวจสอบให้แน่ใจว่า [ปลั๊กอิน BrokerPlugin AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ไม่ถูกบล็อกโดยแอปพลิเคชันหรือไฟร์วอลล์/โปรแกรมป้องกันไวรัส
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office ๒๐๑๖รุ่น16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)