---
title: ประเมินสภาพแวดล้อมเบราว์เซอร์ที่มีอยู่ของคุณและกําหนดเป้าหมาย
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: ff965b3f2fd747763185fcf4cd43479b1cd7189ed737005c2aca4a723df135cb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043675"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>ประเมินสภาพแวดล้อมเบราว์เซอร์ที่มีอยู่ของคุณและกําหนดเป้าหมาย

สละเวลาเพื่อเข้าใจสถานะเบราว์เซอร์และวิสัยทัศน์ของโครงการในปัจจุบันของคุณ เพื่อให้แน่ใจว่าผู้เกี่ยวข้องของโครงการทั้งหมดจะถูกจัดแนวและสอดคล้องกับเป้าหมายเดียวกัน ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. กําหนดสถานะปัจจุบันของคุณ พิจารณาสิ่งต่อไปนี้
- ขณะนี้เบราว์เซอร์ใดที่ปรับใช้ในสภาพแวดล้อมของคุณ
- เบราว์เซอร์ใดที่ถูกตั้งค่าเป็นเบราว์เซอร์เริ่มต้น
- คุณต้องใช้ Internet Explorer ในแอปบางแอปหรือไม่
- คุณใช้รายการไซต์โหมดองค์กรเพื่อกําหนดค่า Internet Explorer ในปัจจุบันหรือไม่
- แพลตฟอร์ม OS ใด เช่น Windows 10 macOS สภาพแวดล้อมของคุณสนับสนุนหรือไม่
- คุณใช้เครื่องมือการจัดการใดในการจัดการเบราว์เซอร์
- ใครรับผิดชอบในการกําหนดค่าและการจัดการเบราว์เซอร์หรือไม่
- กระบวนการในการตรวจสอบความถูกต้องของความเข้ากันได้ของเบราว์เซอร์คืออะไร
2. กําหนดเป้าหมายเพื่อการปรับใช้ของคุณ โปรดระลึกถึงสิ่งต่างๆ ต่อไปนี้
- คุณต้องการตั้งค่าให้[Microsoft Edgeเบราว์เซอร์เริ่มต้นของคุณหรือไม่](https://docs.microsoft.com/DeployEdge/edge-default-browser)
- คุณต้องการซ่อนเวอร์ชันดั้งเดิมของMicrosoft Edgeหรือคุณต้องการปล่อยให้[พร้อมใช้งานให้ผู้ใช้](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)ใช้งานหรือไม่
- คุณจะกําหนด[ค่าMicrosoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)ได้อย่างไร
- ฟีเจอร์ใดที่มีความร้ายแรงในการกําหนดค่าเป็นส่วนหนึ่งของการปรับใช้ครั้งแรกของคุณ
- กระบวนการในการระบุปัญหาความเข้ากันได้หรือการกําหนดค่าที่ระบุคืออะไร
3. เข้าใจเบื้องต้นของฟีเจอร์ที่คุณอาจต้องการใช้ เช่น
- [Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [โหมด Internet Explorer](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [การรับรองความถูกต้องและการซิงค์](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

หลังจากเสร็จสิ้นขั้นตอนเหล่านี้แล้ว คุณก็พร้อมที่จะเริ่มวางแผนกลยุทธ์การปรับใช้ของคุณ
