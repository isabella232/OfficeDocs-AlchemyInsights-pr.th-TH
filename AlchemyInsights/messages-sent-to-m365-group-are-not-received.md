---
title: สมาชิกทุกคนไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480702"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>สมาชิกทุกคนไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365

ตรวจสอบให้แน่ใจว่าสมาชิกทุกคนในกลุ่มได้สมัครใช้งานเพื่อรับอีเมล ดู[ติดตามกลุ่ม ใน Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)  

เมื่อต้องการตรวจสอบสถานะข้อความของสมาชิกที่สมัครใช้งานอีเมลกลุ่ม ให้เรียกใช้การสั่งต่อไปนี้บน[EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อกําหนดค่าสมาชิกกลุ่มทั้งหมดเพื่อรับอีเมลที่ส่งไปยังกลุ่ม Microsoft 365 ในกล่องจดหมายเข้าของพวกเขา:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

ตัวอย่างเช่น:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`