---
title: การแก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664945"
---
# <a name="troubleshoot-password-synchronization"></a>การแก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน

เมื่อต้องการแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านให้เริ่มต้นโดยใช้การแก้ไขปัญหา AAD เชื่อมต่อนี้เพื่อกำหนดว่าทำไมรหัสผ่านจึงไม่ได้รับการซิงค์ เมื่อต้องการเริ่มต้นให้ไปที่[จัดการการซิงค์โดยตรง](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์ Azure AD Connect ของคุณแล้วเลือกตัวเลือก**เรียกใช้ในฐานะผู้ดูแลระบบ**

2. เรียกใช้การตั้งค่า-ExecutionPolicy RemoteSigned หรือตั้งค่า ExecutionPolicy ไม่จำกัด

3. เริ่มตัวช่วยสร้างการเชื่อมต่อ AD Azure

4. ไปที่หน้างานเพิ่มเติม >**แก้ไขปัญหา**  >  **ถัดไป**

5. เลือก **เปิด** ใช้เพื่อเปิดเมนูการแก้ไขปัญหา PowerShell

6. เลือก**แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน**

    ปัญหานี้มักจะเป็นการซิงโครไนซ์รหัสผ่านสำหรับบัญชีผู้ใช้ที่เฉพาะเจาะจง

    **บันทึกย่อ** การซิงโครไนซ์รหัสผ่านล้มเหลวถ้าการซิงค์รหัสผ่านที่เสร็จสมบูรณ์ล่าสุดเป็นเวลาที่แล้ว

สำหรับความช่วยเหลือเพิ่มเติมในการแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านให้ดู[แก้ไขปัญหาการซิงโครไนซ์แฮชของรหัสผ่านด้วย AZURE AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)