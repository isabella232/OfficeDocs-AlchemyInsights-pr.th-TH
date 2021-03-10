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
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694819"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>ประเมินสภาพแวดล้อมเบราว์เซอร์ที่มีอยู่ของคุณและกําหนดเป้าหมาย

การสละเวลาเพื่อเข้าใจสถานะเบราว์เซอร์และการมองเห็นโครงการปัจจุบันของคุณเพื่อให้แน่ใจว่าผู้เกี่ยวข้องของโครงการทั้งหมดจะถูกจัดแนวและอยู่ในเป้าหมายเดียวกัน ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. กําหนดสถานะปัจจุบันของคุณ พิจารณาสิ่งต่อไปนี้
- ขณะนี้เบราว์เซอร์ใดที่ปรับใช้ในสภาพแวดล้อมของคุณ
- เบราว์เซอร์ใดที่ถูกตั้งค่าเป็นเบราว์เซอร์เริ่มต้น
- คุณต้องใช้ Internet Explorer กับแอปบางแอปของคุณหรือไม่
- คุณใช้รายการไซต์โหมดองค์กรเพื่อกําหนดค่า Internet Explorer ในปัจจุบันหรือไม่
- แพลตฟอร์ม OS ใด เช่น Windows 10 และ macOS สภาพแวดล้อมของคุณสนับสนุนหรือไม่
- คุณใช้เครื่องมือการจัดการใดในการจัดการเบราว์เซอร์
- ใครมีหน้าที่รับผิดชอบในการกําหนดค่าและการจัดการเบราว์เซอร์
- กระบวนการตรวจสอบความถูกต้องของความเข้ากันได้ของเบราว์เซอร์คืออะไร
2. กําหนดเป้าหมายเพื่อการปรับใช้ของคุณ โปรดระลึกถึงสิ่งต่างๆ ต่อไปนี้:
- คุณต้องการตั้งค่า Microsoft [Edge เป็นเบราว์เซอร์เริ่มต้น](https://docs.microsoft.com/DeployEdge/edge-default-browser)ของคุณหรือไม่
- คุณต้องการซ่อนเวอร์ชันดั้งเดิมของ Microsoft Edge หรือคุณต้องการปล่อยให้ [พร้อมใช้งานกับผู้ใช้](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)หรือไม่
- คุณจะกําหนด [ค่า Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)อย่างไร
- ฟีเจอร์ใดที่มีความร้ายแรงในการกําหนดค่าให้เป็นส่วนหนึ่งของการปรับใช้ครั้งแรกของคุณ
- กระบวนการในการระบุปัญหาความเข้ากันได้หรือการกําหนดค่าที่ระบุคืออะไร
3. เข้าใจเบื้องต้นของฟีเจอร์ที่คุณอาจต้องการใช้ เช่น
- [Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [โหมด Internet Explorer](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [การรับรองความถูกต้องและการซิงค์](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

หลังจากเสร็จสิ้นขั้นตอนเหล่านี้แล้ว คุณก็พร้อมที่จะเริ่มวางแผนกลยุทธ์การปรับใช้
