---
title: ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM for a specific domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749733"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM for a specific domain

ถ้าคุณไม่สามารถสร้างระเบียน DNS ของ DKIM ในศูนย์การจัดการ ให้ลองใช้ Exchange Online PowerShell 

เมื่อต้องการสร้างระเบียน DNS DKIM โดยใช้ Exchange Online PowerShell ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. เปิด Windows PowerShell ในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในลดับที่อธิบายไว้:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
ถ้าคุณมีปัญหาในการเชื่อมต่อกับ Exchange Online PowerShell ให้ดู[เชื่อมต่อกับ Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. เมื่อคุณเชื่อมต่อกับ Exchange Online PowerShell ให้เรียกใช้การสั่งต่อไปนี้:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. เมื่อเรียกใช้การสั่งข้างต้นเสร็จสมบูรณ์แล้ว ให้เรียกใช้สั่งต่อไปนี้เพื่อสิ้นสุดเซสชัน Exchange Online PowerShell:

    `Remove-PSSession $Session` 



