---
title: แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105797"
---
# <a name="troubleshoot-password-synchronization"></a>แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน

เมื่อต้องการแก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน ให้เริ่มโดยใช้ AAD เชื่อมต่องานการแก้ไขปัญหาเพื่อระบุสาเหตุที่รหัสผ่านไม่ซิงค์ เมื่อต้องการเริ่ม ให้ไปที่ [จัดการการซิงค์](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)โดยตรง  

1. เปิดเซสชันWindows PowerShellใหม่บนเซิร์ฟเวอร์ Azure AD เชื่อมต่อ และ **เลือกตัวเลือก เรียกใช้** ในฐานะผู้ดูแลระบบ

2. เรียกใช้ Set-ExecutionPolicy RemoteSigned หรือ Set-ExecutionPolicy Unrestricted

3. เริ่มตัวช่วยสร้างการเชื่อมต่อ Azure AD

4. ไปที่หน้า งานเพิ่มเติม >  >  **แก้ไขปัญหา** ถัดไป

5. เลือกเปิดใช้ เพื่อเปิดเมนู การแก้ไขปัญหา PowerShell

6. เลือก **แก้ไขปัญหาการซิงโครไนซ์** รหัสผ่าน

    ปัญหามักจะเป็นรหัสผ่านที่ไม่ได้ซิงโครไนซ์กับบัญชีผู้ใช้ที่ระบุ

    **หมายเหตุ** การซิงโครไนซ์รหัสผ่านล้มเหลวถ้าช่วงเวลาที่ผ่านมาการซิงค์รหัสผ่านประสบความสาเร็จล่าสุด

For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD เชื่อมต่อ sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).