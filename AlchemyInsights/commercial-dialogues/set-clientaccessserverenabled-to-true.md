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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749974"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ตั้งค่า ClientAccessServerEnabled เป็น True

ถ้าคุณไม่สามารถเปิดข้อความอีเมลที่เข้ารหัสลับ และดูสิ่งที่แนบมา **แบบ rpmsg** แทน ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. เชื่อมต่อกับ Exchange Online PowerShell

> [!NOTE]
> เมื่อต้องการเชื่อมต่อกับ Exchange Online PowerShell คุณต้องลงชื่อเข้าใช้โดยใช้ผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบ Exchange

   a. เปิด Windows PowerShell แล้วเรียกใช้การสั่งต่อไปนี้: `$UserCredential = Get-Credential`
b. ในกล่องโต้ตอบการร้องขอ **ข้อมูลรับรองความถูกต้องของ Windows PowerShell** ให้ใส่บัญชีและรหัสผ่านของที่โรงเรียนหรือที่โรงเรียนของคุณ คลิก **OK** 

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

