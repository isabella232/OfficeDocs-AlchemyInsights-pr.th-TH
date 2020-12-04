---
title: แก้ไขปัญหา .PRT
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573903"
---
# <a name="troubleshoot-prt-issue"></a>แก้ไขปัญหา .PRT

สำหรับอุปกรณ์ใดก็ตามที่ต้องการรับการรับรองความถูกต้องจะต้องมีการลงทะเบียนทั้งหมดและในสถานะที่ดีและสามารถรับโทเค็นการรีเฟรชหลัก (.PRT) ได้

กระบวนการลงทะเบียนการเข้าร่วม AD Azure แบบไฮบริดจำเป็นต้องมีอุปกรณ์ที่จะอยู่บนเครือข่ายขององค์กร นอกจากนี้ยังทำงานผ่าน VPN แต่มีเตือนบางอย่างที่มีอยู่ เราเคยได้ยินลูกค้าจำเป็นต้องมีความช่วยเหลือเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนการเข้าร่วม AD Azure ของไฮบริดภายใต้สถานการณ์การทำงานระยะไกล ต่อไปนี้เป็นรายละเอียดของสิ่งที่เกิดขึ้น ' ภายใต้เครื่องดูดควัน ' ในระหว่างขั้นตอนการลงทะเบียน

**สภาพแวดล้อมการรับรองความถูกต้องของระบบคลาวด์ (โดยใช้การซิงค์แฮชของรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส**

ขั้นตอนการลงทะเบียนนี้เรียกว่า "การเข้าร่วมการซิงค์"

1. Windows 10 จะค้นพบระเบียน SCP เมื่อผู้ใช้เข้าสู่ระบบไปยังอุปกรณ์
    1. อุปกรณ์แรกพยายามเรียกข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] สำหรับข้อมูลเพิ่มเติมให้ดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)นี้
    2. ถ้าล้มเหลวอุปกรณ์จะสื่อสารกับ Active directory ภายในองค์กร (AD) เพื่อรับข้อมูลผู้เช่าจากจุดเชื่อมต่อบริการ (SCP) เมื่อต้องการตรวจสอบ SCP โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้ 

> [!NOTE]
> เราขอแนะนำให้ทำการเปิดใช้งาน SCP ในโฆษณาและใช้การตรวจสอบความถูกต้องของการเริ่มต้นที่ด้านไคลเอ็นต์

2. Windows 10 พยายามสื่อสารกับ Azure AD ภายใต้บริบทของระบบเพื่อรับรองความถูกต้องของตัวเองจาก Azure AD คุณสามารถตรวจสอบว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีผู้ใช้ของระบบโดยใช้สคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์ทดสอบ

3. Windows 10 จะสร้างใบรับรองที่เซ็นชื่อด้วยตนเองและจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ในโฆษณาภายในองค์กร สิ่งนี้จำเป็นต้องใช้ตัวควบคุมโดเมนในสาย

4. วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่าน Azure AD Connect การซิงค์วงจรคือทุกๆ30นาทีตามค่าเริ่มต้นแต่จะขึ้นอยู่กับการกำหนดค่าของ Azure AD Connect สำหรับข้อมูลเพิ่มเติมโปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)นี้

5. ในขั้นตอนนี้คุณควรจะสามารถเห็นอุปกรณ์เรื่องในสถานะ "ค้างอยู่" ภายใต้ใบพัดของอุปกรณ์ของ Azure Portal

6. ที่ผู้ใช้ถัดไปเข้าสู่ระบบ Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์ 

> [!NOTE]
> ถ้าคุณอยู่ใน VPN และกระบวนการออกจากระบบ-การเข้าสู่ระบบจะสิ้นสุดลงการเชื่อมต่อโดเมนคุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเองได้:
 1. ออกจาก dsregcmd/join ภายในเครื่องบนพร้อมท์ของผู้ดูแลระบบหรือจากระยะไกลผ่าน PSExec ไปยังพีซีของคุณ ตัวอย่างเช่น PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาการรวมแบบไฮบริดให้ดูที่[แก้ไขปัญหาเกี่ยวกับอุปกรณ์](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
