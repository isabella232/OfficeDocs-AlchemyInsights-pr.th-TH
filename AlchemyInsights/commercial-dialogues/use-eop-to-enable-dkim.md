---
title: ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM ให้กับโดเมนที่ระบุ
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070343"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>ใช้ Exchange Online PowerShell เพื่อเปิดใช้งาน DKIM ให้กับโดเมนที่ระบุ

ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ในศูนย์การจัดการ ให้ลองใช้ Exchange Online PowerShell 

เมื่อต้องการสร้างระเบียน DNS ของ DKIM Exchange Online PowerShell ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. เปิดWindows PowerShellในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในลดับที่อธิบายไว้

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
ถ้าคุณมีปัญหาในการเชื่อมต่อกับ Exchange Online PowerShell ให้ดูที่[เชื่อมต่อ Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. เมื่อคุณเชื่อมต่อกับ PowerShell Exchange Onlineเรียกใช้การสั่งต่อไปนี้:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. เมื่อเรียกใช้การสั่งข้างต้นเสร็จสมบูรณ์แล้ว ให้เรียกใช้สั่งต่อไปนี้เพื่อสิ้นสุดเซสชัน Exchange Online PowerShell:

    `Remove-PSSession $Session` 



