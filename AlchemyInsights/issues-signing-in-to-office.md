---
title: ปัญหาในการลงชื่อเข้าใช้Microsoft 365แอป
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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088055"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>หน้าจอลงชื่อเข้าใช้ว่างเปล่าในMicrosoft 365แอป

เมื่อต้องการแก้ไขปัญหานี้ ให้ลองวิธีต่อไปนี้:
- ติดตั้งการอัปเดตล่าสุด[Windowsและ](https://support.microsoft.com/help/4027667/windows-10-update)[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- ตั้งค่าตัวเลือก Internet Explorer ใหม่:**ไปที่** เครื่องมือ ตัวเลือกอินเทอร์เน็ต ตั้งค่าใหม่การตั้งค่า Internet Explorer ขั้นสูง (โปรดทราบว่า คุณจะสูญเสียการตั้งค่าแบบปรับแต่งเอง) แล้วลองลงชื่อเข้าใช้  >    >    >  Officeอีกครั้ง
- ปิดใช้งานโปรแกรมWindows Defender Application Guard (WDAG) หรือไฟร์วอลล์หรือโปรแกรมป้องกันไวรัสที่คล้ายกัน:
    1. ใน แผงควบคุม **ให้ไปที่** โปรแกรม แล้วเลือก **Windowsเปิดหรือปิดฟีเจอร์**
    2. ถ้าคุณWindows Defender Application Guardให้ใช้งาน ให้ลองปิดใช้งาน<br/>
    **หมายเหตุ:** คุณอาจต้องรีสตาร์ตคอมพิวเตอร์
- ตรวจสอบให้แน่ใจว่าปลั๊กอิน [AAD WAM ของ](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft.AAD.BrokerPlugin จะไม่ถูกบล็อกโดยแอปพลิเคชันหรือไฟร์วอลล์/โปรแกรมป้องกันไวรัส
- [ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows<br/>
    **หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว (เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)

For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).