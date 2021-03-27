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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398748"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ

Microsoft Edge ใช้บัญชีเริ่มต้นของ OS เพื่อลงชื่อเข้าใช้ผู้ใช้โดยอัตโนมัติตามวิธีกําหนดค่าอุปกรณ์ของผู้ใช้ 

สถานการณ์สมมติของการกําหนดค่าอุปกรณ์แต่ละชนิดและขั้นตอนการลงชื่อเข้าใช้ของผู้ใช้ที่ไม่เป็นอิสระมีอธิบายไว้ด้านล่าง:

- **อุปกรณ์นี้เป็นแบบไฮบริด/AAD-J:** ตัวเลือกนี้จะพร้อมใช้งานบน Windows 10, Windows ระดับลง และเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน ผู้ใช้จะลงชื่อเข้าใช้ด้วยบัญชี Azure Active Directory (AD) ของพวกเขาโดยอัตโนมัติ
- **อุปกรณ์ถูกรวมโดเมน**: ตัวเลือกนี้จะพร้อมใช้งานบน Windows 10, Windows ระดับลง และเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน ตามค่าเริ่มต้น ผู้ใช้ที่มีบัญชีผู้ใช้โดเมนจะไม่ลงชื่อเข้าใช้โดยอัตโนมัติ เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้อัตโนมัติให้กับพวกเขา ให้ใช้นโยบาย **ConfigureOnPremisesAccountAutoSignIn** เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้อัตโนมัติให้กับผู้ใช้ที่มีบัญชี Azure AD ให้พิจารณาการเข้าร่วมอุปกรณ์แบบไฮบริด
- **บัญชีเริ่มต้นของระบบปฏิบัติการ** คือบัญชี Microsoft : ตัวเลือกนี้จะพร้อมใช้งานใน Windows 10 RS3 (เวอร์ชัน 1709 รุ่น 10.0.16299) และเวอร์ชันที่ใหม่กว่า สถานการณ์ไม่น่าเกิดขึ้นบนอุปกรณ์ขององค์กร แต่ถ้าบัญชีเริ่มต้นของ OS เป็นบัญชี Microsoft แล้ว Microsoft Edge จะลงชื่อเข้าใช้ผู้ใช้ด้วยบัญชี Microsoft โดยอัตโนมัติ
 
 
