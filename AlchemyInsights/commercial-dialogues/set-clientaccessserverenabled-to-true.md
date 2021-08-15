---
title: ตั้งค่า ClientAccessServerEnabled เป็น True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994884"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ตั้งค่า ClientAccessServerEnabled เป็น True

ถ้าคุณไม่สามารถเปิดข้อความอีเมลที่เข้ารหัสลับ และดูสิ่งที่แนบมา **แบบ rpmsg** แทน ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. เชื่อมต่อ Exchange Online PowerShell

> [!NOTE]
> เมื่อต้องการเชื่อมต่อกับ Exchange Online PowerShell คุณต้องลงชื่อเข้าใช้โดยใช้ผู้ดูแลระบบส่วนกลางหรือExchangeผู้ดูแลระบบของคุณ

   a. เปิด Windows PowerShell แล้วเรียกใช้การสั่งต่อไปนี้:`$UserCredential = Get-Credential`
b. ในกล่องโต้ตอบ **Windows PowerShellการร้องขอข้อมูลของฉัน** ให้ใส่บัญชีและรหัสผ่านของที่โรงเรียนหรือที่โรงเรียนของคุณ คลิก **OK** 

2. เรียกใช้การสั่งต่อไปนี้เพื่อสร้างเซสชันใหม่:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. เรียกใช้คำสั่งต่อไปนี้:
    
    `Import-PSSession $Session -DisableNameChecking`

3. เรียกใช้ `Get-IRMConfiguration` การสั่ง

4. ตรวจสอบ **การตั้งค่า ClientAccessServerEnabled** 

    a. ถ้า **การตั้งค่า ClientAccessServerEnabled** ถูกตั้งค่า **เป็น False** ให้เรียกใช้ cmdlet ต่อไปนี้: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> ปิดเซสชัน PowerShell ของคุณเสมอด้วยสั่งต่อไปนี้: `Remove-PSSession $Session`

For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

