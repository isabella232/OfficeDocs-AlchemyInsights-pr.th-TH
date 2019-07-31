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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938367"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>เครื่องหมายในหน้าจอว่างในโปรแกรมประยุกต์ของ Office

เมื่อต้องการแก้ไขปัญหานี้ ลองต่อไปนี้:
- ติดตั้งโปรแกรมปรับปรุงล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- รีเซ็ตตัวเลือก Internet Explorer: ไปที่**เครื่องมือ** > **ตัวเลือกอินเทอร์เน็ต** > **ขั้นสูง** > **ตั้งค่า Internet Explorer** (โปรดสังเกตว่า คุณจะสูญเสียการตั้งค่าแบบกำหนดเอง), แล้วลองลงชื่อเข้าใช้ให้กับสำนักงานอีกครั้ง
- ปิดการใช้งาน Windows Defender โปรแกรมประยุกต์ Guard (WDAG) หรือโปรแกรมไฟร์วอลล์หรือโปรแกรมป้องกันไวรัสใด ๆ คล้ายกัน:
    1. ใน'แผงควบคุม' ไปยัง**โปรแกรม**และจากนั้น เลือก**เปิด หรือปิดคุณลักษณะของ Windows ที่เปิดใช้งาน**
    2. ถ้าเปิดใช้งาน Windows Guard แอพลิเคชันของ Defender ลองปิดใช้งาน<br/>
    **หมายเหตุ:** คุณอาจต้องรีสตาร์ทเครื่องคอมพิวเตอร์
- ให้แน่ใจว่า Microsoft.AAD.BrokerPlugin [WAM AAD ปลั๊กอิน](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)ไม่ถูกบล็อก โดยโปรแกรมประยุกต์หรือไฟร์ วอลล์/anti-virus โปรแกรมใด ๆ
- [ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0 (แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)

สำหรับข้อมูลเพิ่มเติม ดู[ปัญหาการเชื่อมต่อในเครื่องหลังจากการปรับปรุง Office 2016 build 16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)