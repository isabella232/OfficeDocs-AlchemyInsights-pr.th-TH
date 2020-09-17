---
title: ไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft ๓๖๕โดยสมาชิกทั้งหมด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806166"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>ไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft ๓๖๕โดยสมาชิกทั้งหมด

ตรวจสอบให้แน่ใจว่าสมาชิกกลุ่มทั้งหมดได้รับการสมัครใช้งานเพื่อรับอีเมลดังกล่าว ให้ดู[ที่ติดตามกลุ่มใน Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)  

เมื่อต้องการตรวจสอบสถานะข้อความของสมาชิกที่ได้สมัครใช้งานอีเมลของกลุ่มให้เรียกใช้คำสั่งต่อไปนี้บน [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`