---
title: ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678818"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ

Microsoft Edge ใช้บัญชีเริ่มต้นของระบบปฏิบัติการเพื่อลงชื่อเข้าใช้โดยอัตโนมัติตามวิธีที่อุปกรณ์ของผู้ใช้ได้รับการกำหนดค่า 

สถานการณ์สมมติของการกำหนดค่าอุปกรณ์แต่ละชนิดและกระบวนการลงชื่อเข้าใช้ของผู้ใช้ที่ขึ้นต่อกันจะอธิบายไว้ด้านล่าง:

1. **อุปกรณ์คือไฮบริด/AAD-J**: ตัวเลือกนี้จะพร้อมใช้งานบน windows 10, windows ระดับล่างและเวอร์ชันของเซิร์ฟเวอร์ที่สอดคล้องกัน ผู้ใช้จะได้รับการลงชื่อเข้าใช้โดยอัตโนมัติด้วยบัญชีผู้ใช้ Azure Active directory (AD)
2. **อุปกรณ์มีการเข้าร่วมโดเมน**: ตัวเลือกนี้จะพร้อมใช้งานบน windows 10, windows ระดับล่างและเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน ตามค่าเริ่มต้นผู้ใช้ที่มีบัญชีโดเมนไม่ได้ลงชื่อเข้าใช้โดยอัตโนมัติ เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้โดยอัตโนมัติให้ใช้นโยบาย **ConfigureOnPremisesAccountAutoSignIn** เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้โดยอัตโนมัติสำหรับผู้ใช้ที่มีบัญชีผู้ใช้ AD Azure ให้ลองใช้การเข้าร่วมอุปกรณ์ของพวกเขา
3. **บัญชีเริ่มต้นของระบบปฏิบัติการคือบัญชี Microsoft**: ตัวเลือกนี้จะพร้อมใช้งานบน WINDOWS 10 ขี่ (เวอร์ชัน๑๗๐๙, รุ่น 10.0.16299) และเวอร์ชันที่ใหม่กว่า สถานการณ์สมมติไม่น่าจะเกิดขึ้นบนอุปกรณ์ขององค์กร อย่างไรก็ตามถ้าบัญชีเริ่มต้นของระบบปฏิบัติการเป็นบัญชี Microsoft microsoft Edge จะลงชื่อเข้าใช้โดยอัตโนมัติในผู้ใช้ด้วยบัญชี Microsoft
 
 
