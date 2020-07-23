---
title: การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387896"
---
# <a name="troubleshoot-password-synchronization"></a>การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน

เมื่อต้องการแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน ให้เริ่มโดยใช้งานการแก้ไขปัญหาการเชื่อมต่อ AAD นี้เพื่อตรวจสอบว่าเหตุใดรหัสผ่านจึงไม่ซิงค์ เมื่อต้องการเริ่มต้น ให้ไปที่[จัดการการซิงค์โดยตรง](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์เชื่อมต่อโฆษณา Azure ของคุณ และเลือกตัวเลือก**เรียกใช้ในฐานะผู้ดูแลระบบ**

2. เรียกใช้ชุดการดําเนินการระยะไกลPolicyหรือตั้งค่า-ExecutionPolicyไม่จํากัด

3. เริ่มตัวช่วยสร้างการเชื่อมต่อโฆษณา Azure

4. ไปที่หน้า งานเพิ่มเติม >**แก้ไขปัญหา**  >  **ถัดไป**

5. เลือก**เปิดใช้**เพื่อเปิดเมนูการแก้ไขปัญหา PowerShell

6. เลือก**แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน**

    ปัญหานี้มักจะว่า รหัสผ่านจะไม่ซิงโครไนส์สําหรับบัญชีผู้ใช้ที่ระบุ

    **หมายเหตุ** การซิงโครไนส์รหัสผ่านล้มเหลวถ้าการซิงค์รหัสผ่านที่สําเร็จครั้งล่าสุดคือเวลาที่ผ่านมา

สําหรับความช่วยเหลือเพิ่มเติมการแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน ให้ดูที่[การแก้ไขปัญหาการซิงโครไนส์แฮชรหัสผ่านด้วยการซิงค์การเชื่อมต่อ AD Azure](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)