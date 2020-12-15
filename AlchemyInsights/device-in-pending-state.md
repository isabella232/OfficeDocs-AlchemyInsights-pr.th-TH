---
title: อุปกรณ์ในสถานะที่ค้างอยู่
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679994"
---
# <a name="device-in-pending-state"></a>อุปกรณ์ในสถานะที่ค้างอยู่

**เบื้อง**

1. ถ้าคุณกำลังตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรกโปรดตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน [บทนำสู่การจัดการอุปกรณ์ใน Azure active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ที่จะแนะนำคุณเกี่ยวกับวิธีการรับอุปกรณ์ภายใต้การควบคุมของ azure AD
2. ถ้าคุณกำลังลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรงและการลงชื่อเข้าใช้ใน Intune คุณจำเป็นต้องตรวจสอบให้แน่ใจว่าคุณได้ [กำหนดค่า intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) และให้ [สิทธิ์](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) การใช้งานเป็นอันดับแรก
3. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดำเนินการในโฆษณา Azure และโฆษณาภายในองค์กร เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าสำหรับการลงทะเบียนอุปกรณ์ได้ นอกจากนี้ถ้าคุณกำลังตั้งค่าการลงทะเบียนอัตโนมัติใน active directory ภายในองค์กรของคุณคุณจะต้องเป็นผู้ดูแลไดเรกทอรีที่ใช้งานอยู่และ FS โฆษณา (ถ้ามี)

กระบวนการลงทะเบียนการเข้าร่วม AD Azure แบบไฮบริดจำเป็นต้องมีอุปกรณ์ที่จะอยู่บนเครือข่ายขององค์กร นอกจากนี้ยังทำงานผ่าน VPN แต่มีเตือนบางอย่างที่มีอยู่ เราได้ยินลูกค้าที่จำเป็นต้องมีความช่วยเหลือเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนการเข้าร่วม AD Azure ของไฮบริดภายใต้สถานการณ์การทำงานระยะไกล

**สภาพแวดล้อมการรับรองความถูกต้องของระบบคลาวด์ (โดยใช้การซิงค์แฮชของรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส**

ขั้นตอนการลงทะเบียนนี้เรียกว่า "การเข้าร่วมการซิงค์"

ต่อไปนี้เป็นรายละเอียดของสิ่งที่เกิดขึ้นระหว่างขั้นตอนการลงทะเบียน:

1. Windows 10 จะค้นพบระเบียนจุดเชื่อมต่อบริการ (SCP) เมื่อผู้ใช้เข้าสู่ระบบอุปกรณ์

    1. อุปกรณ์แรกพยายามเรียกข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] สำหรับข้อมูลเพิ่มเติมให้ดูที่[เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. ถ้าล้มเหลวอุปกรณ์จะสื่อสารกับไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรเพื่อรับข้อมูลผู้เช่าจาก SCP เมื่อต้องการตรวจสอบ SCP ให้ดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้

    > [!NOTE]
    > เราขอแนะนำให้เปิดใช้งาน SCP ในไดเรกทอรีที่ใช้งานอยู่และใช้ SCP ฝั่งไคลเอ็นต์สำหรับการตรวจสอบความถูกต้องเริ่มต้นเท่านั้น

2. Windows 10 พยายามสื่อสารกับ Azure AD ภายใต้บริบทของระบบเพื่อรับรองความถูกต้องของตัวเองจาก Azure AD

    คุณสามารถตรวจสอบว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีผู้ใช้ของระบบโดยใช้[สคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์ทดสอบ](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 จะสร้างใบรับรองที่เซ็นชื่อด้วยตนเองและจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ในไดเรกทอรีที่ใช้งานอยู่ภายในองค์กร สิ่งนี้จำเป็นต้องใช้ตัวควบคุมโดเมนในสาย

4. วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่าน Azure AD Connect การซิงค์วงจรคือทุกๆ30นาทีตามค่าเริ่มต้นแต่จะขึ้นอยู่กับการกำหนดค่าของ Azure AD Connect สำหรับข้อมูลเพิ่มเติมโปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)นี้

5. ในขั้นตอนนี้คุณควรจะสามารถเห็นอุปกรณ์เรื่องในสถานะ "**ค้างอยู่**" ภายใต้ใบพัดของอุปกรณ์ของ Azure Portal

6. ที่ผู้ใช้ถัดไปเข้าสู่ระบบ Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์

    > [!NOTE]
    > ถ้าคุณอยู่ใน VPN และออกจากระบบ/การเข้าสู่ระบบจะสิ้นสุดการเชื่อมต่อโดเมนคุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเองได้ เมื่อต้องการทำสิ่งต่อไปนี้:
    >
    > ออกจาก `dsregcmd /join` พร้อมท์ภายในเครื่องของผู้ดูแลระบบหรือจากระยะไกลผ่านทาง PSExec ไปยังพีซีของคุณ
    >
    > ตัวอย่างเช่น: `PsExec -s \\win10client01 cmd, dsregcmd /join`

สำหรับปัญหาทั่วไปเกี่ยวกับการลงทะเบียนอุปกรณ์ของ Azure Active directory ให้ดูที่คำ[ถามที่ถามบ่อยเกี่ยวกับอุปกรณ์](https://docs.microsoft.com/azure/active-directory/devices/faq)
