---
title: สมาชิกทุกคนMicrosoft 365ไม่ได้รับข้อความที่ส่งถึงกลุ่ม
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976524"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>สมาชิกทุกคนไม่ได้รับMicrosoft 365ส่งข้อความถึงกลุ่มที่ถูกส่งถึง

ตรวจสอบให้แน่ใจว่าสมาชิกกลุ่มทุกคนได้สมัครใช้งานเพื่อรับอีเมล ดู[ติดตามกลุ่มใน Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)  

เมื่อต้องการตรวจสอบสถานะข้อความของสมาชิกที่สมัครใช้งานอีเมลกลุ่ม ให้เรียกใช้การสั่งต่อไปนี้บน[EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อกําหนดค่าสมาชิกกลุ่มทั้งหมดเพื่อรับอีเมลที่Microsoft 365กลุ่มในกล่องจดหมายเข้าของพวกเขา:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

ตัวอย่างเช่น:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`