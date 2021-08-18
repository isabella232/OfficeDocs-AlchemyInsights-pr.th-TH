---
title: แก้ไขปัญหา PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330978"
---
# <a name="troubleshoot-prt-issue"></a>แก้ไขปัญหา PRT

เพื่อให้อุปกรณ์ใดๆ ได้รับการรับรองความถูกต้องให้เสร็จสมบูรณ์ อุปกรณ์ต้องได้รับการลงทะเบียนอย่างสมบูรณ์และอยู่ในสถานะที่ดี และสามารถรับโทเค็นรีเฟรชหลัก (PRT) ได้

กระบวนการลงทะเบียนการเข้าร่วม Azure AD แบบไฮบริดต้องการให้อุปกรณ์อยู่บนเครือข่ายขององค์กร และยังใช้งานได้ผ่าน VPN แต่ก็มีบางสิ่งที่ต้องค่ําคาม เราทราบถึงลูกค้าที่ต้องการความช่วยเหลือเกี่ยวกับการแก้ไขปัญหากระบวนการลงทะเบียนเข้าร่วม Azure AD แบบไฮบริดภายใต้สถานการณ์การงานระยะไกล ต่อไปนี้คือข้อมูลแยกย่อยของสิ่งที่เกิดขึ้น 'ภายใต้เครื่องแบบเดียวกัน' ในระหว่างกระบวนการลงทะเบียน

**สภาพแวดล้อมการรับรองความถูกต้องระบบคลาวด์ (ใช้การซิงค์แฮชรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส-ผ่าน)**

โฟลว์การลงทะเบียนนี้เรียกอีกอย่างว่า "ซิงค์การเข้าร่วม"

1. Windows 10ระเบียน SCP เมื่อผู้ใช้เข้าสู่ระบบอุปกรณ์
    1. อุปกรณ์พยายามดึงข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] ก่อน หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)นี้
    2. ถ้าล้มเหลว อุปกรณ์จะสื่อสารกับ Active Directory (AD) ภายในองค์กรเพื่อรับข้อมูลผู้เช่าจากจุดเชื่อมต่อบริการ (SCP) เมื่อต้องการตรวจสอบ SCP โปรดดูที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้ 

**หมายเหตุ**: เราขอแนะนนะให้เปิดใช้งาน SCP ใน AD และใช้ SCP ฝั่งไคลเอ็นต์เพื่อการตรวจสอบความถูกต้องเริ่มต้นเท่านั้น

2. Windows 10พยายามสื่อสารกับ Azure AD ภายใต้บริบทระบบเพื่อรับรองความถูกต้องตัวเองกับ Azure AD คุณสามารถตรวจสอบได้ว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีระบบโดยใช้สคริปต์ทดสอบการเชื่อมต่อการลงทะเบียนอุปกรณ์หรือไม่

3. Windows 10จะสร้างใบรับรองที่ลงนามด้วยตนเองและจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ใน AD ภายในองค์กร การนี้ต้องใช้การเชื่อมต่อแบบบรรทัด -of-sight ไปยังตัวควบคุมโดเมน

4. วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่านทางเชื่อมต่อ Azure AD รอบการซิงค์คือทุกๆ 30 นาทีตามค่าเริ่มต้น แต่ขึ้นอยู่กับการกําหนดค่า Azure AD เชื่อมต่อ หากต้องการข้อมูลเพิ่มเติม โปรดดูที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)นี้

5. ในขั้นตอนนี้ คุณควรจะสามารถดูอุปกรณ์หัวข้อในสถานะ "รอการพิจารณา" ภายใต้ ใบอุปกรณ์ ของพอร์ทัล Azure

6. เมื่อผู้ใช้ถัดไปลงชื่อเข้าใช้Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์ 

**หมายเหตุ**: ถ้าคุณใช้ VPN และกระบวนการเข้าสู่ระบบด้วยโลโก้จะสิ้นสุดการเชื่อมต่อโดเมน คุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเอง:
 1. ออก dsregcmd /join ภายในเครื่องบนพร้อมท์ของผู้ดูแลระบบหรือระยะไกลผ่าน PSExec ไปยังพีซีของคุณ ตัวอย่างเช่น PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
