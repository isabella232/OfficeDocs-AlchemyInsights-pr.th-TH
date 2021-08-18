---
title: อุปกรณ์อยู่ในสถานะที่ค้างอยู่
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
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330391"
---
# <a name="device-in-pending-state"></a>อุปกรณ์อยู่ในสถานะที่ค้างอยู่

**เงื่อนไขเบื้องต้น:**

1. ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก โปรดตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน บทนําสู่การจัดการอุปกรณ์ใน Azure Active Directory [(Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support)ที่จะแนะนําวิธีรับอุปกรณ์ภายใต้การควบคุมของ Azure AD
2. หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์เหล่านั้นใน Intuned คุณจะต้องตรวจสอบให้แน่ใจว่า คุณได้กําหนดค่า[Intuned](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)[และได้](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)ให้สิทธิ์การใช้งานก่อน
3. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD และ AD ภายในองค์กร เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้ นอกจากนี้ ถ้าคุณตั้งค่าการลงทะเบียนอัตโนมัติใน Active Directory ภายในองค์กรของคุณ คุณจะต้องเป็นผู้ดูแลระบบของ Active Directory และ AD FS (ถ้ามี)

กระบวนการลงทะเบียนการเข้าร่วม Azure AD แบบไฮบริดต้องการให้อุปกรณ์อยู่บนเครือข่ายขององค์กร และยังใช้งานได้ผ่าน VPN แต่ก็มีบางสิ่งที่ต้องค่ําคาม เราทราบถึงลูกค้าที่ต้องการความช่วยเหลือเกี่ยวกับการแก้ไขปัญหากระบวนการลงทะเบียนเข้าร่วม Azure AD แบบไฮบริดภายใต้สถานการณ์การงานระยะไกล

**สภาพแวดล้อมการรับรองความถูกต้องระบบคลาวด์ (ใช้การซิงค์แฮชรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส-ผ่าน)**

โฟลว์การลงทะเบียนนี้เรียกอีกอย่างว่า "ซิงค์การเข้าร่วม"

ต่อไปนี้คือข้อมูลแยกย่อยของสิ่งที่เกิดขึ้นในระหว่างกระบวนการลงทะเบียน:

1. Windows 10ระเบียน Service Connection Point (SCP) เมื่อผู้ใช้เข้าสู่ระบบอุปกรณ์

    1. อุปกรณ์พยายามดึงข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] ก่อน ดูข้อมูลเพิ่มเติม [ที่](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)เอกสาร
    1. ถ้าล้มเหลว อุปกรณ์จะสื่อสารกับ Active Directory ภายในองค์กรเพื่อรับข้อมูลผู้เช่าจาก SCP เมื่อต้องการตรวจสอบ SCP ให้ [อ้างอิงเอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้

    **หมายเหตุ**: เราขอแนะนนะให้เปิดใช้งาน SCP ใน Active Directory และใช้ SCP ฝั่งไคลเอ็นต์ในการตรวจสอบความถูกต้องเริ่มต้นเท่านั้น

2. Windows 10พยายามสื่อสารกับ Azure AD ภายใต้บริบทระบบเพื่อรับรองความถูกต้องตัวเองกับ Azure AD

    คุณสามารถตรวจสอบได้ว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีระบบโดยใช้ [สคริปต์ทดสอบการเชื่อมต่อการลงทะเบียน](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)อุปกรณ์หรือไม่

3. Windows 10จะสร้างใบรับรองที่ลงนามด้วยตนเอง และจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ใน Active Directory ภายในองค์กร การนี้ต้องใช้การเชื่อมต่อแบบบรรทัด -of-sight ไปยังตัวควบคุมโดเมน

4. วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่านทางเชื่อมต่อ Azure AD รอบการซิงค์คือทุก 30 นาทีตามค่าเริ่มต้น แต่ขึ้นอยู่กับการกําหนดค่า Azure AD เชื่อมต่อ โปรดดูเอกสารนี้ เพื่อดู[ข้อมูลเพิ่มเติม](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. ในขั้นตอนนี้ คุณควรจะสามารถดูอุปกรณ์หัวข้อในสถานะ " รอ **การ** อยู่ " ภายใต้ ใบอุปกรณ์ ของพอร์ทัล Azure

6. เมื่อผู้ใช้ถัดไปลงชื่อเข้าใช้Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์

    **หมายเหตุ**: ถ้าคุณอยู่บน VPN และ logoff/login จะสิ้นสุดการเชื่อมต่อโดเมน คุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเองได้ วิธีการ:
    
    ออก `dsregcmd /join` การแจ้งเตือนภายในเครื่องบนพร้อมท์ของผู้ดูแลระบบหรือระยะไกลผ่าน PSExec ไปยังพีซีของคุณ\
    ตัวอย่างเช่น: `PsExec -s \\win10client01 cmd, dsregcmd /join`

หากต้องการทราบปัญหาทั่วไปAzure Active Directoryการลงทะเบียนอุปกรณ์ของคุณ โปรดดู บทความ[ที่ถามบ่อยเกี่ยวกับ](https://docs.microsoft.com/azure/active-directory/devices/faq)อุปกรณ์
