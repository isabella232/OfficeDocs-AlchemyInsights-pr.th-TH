---
title: ผู้ส่งไม่ได้รับอีเมลที่ส่งไปยังMicrosoft 365ของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958316"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>ผู้ส่งไม่ได้รับอีเมลที่ส่งไปยังMicrosoft 365ของคุณ

ตามค่าเริ่มต้น ผู้ส่งข้อความอีเมลไปยังกลุ่ม Microsoft 365 จะไม่ได้รับสําเนาของข้อความในกล่องจดหมายเข้าของพวกเขา แม้ว่าผู้ส่งจะเป็นสมาชิกกลุ่ม

ใช้สั่ง EXO PowerShell นี้เพื่อให้ผู้ส่งได้รับสําเนาของแต่ละอีเมลที่พวกเขาส่งไปยังMicrosoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

เมื่อต้องการเปิดใช้งานการตั้งค่ากล่องจดหมายทั้งหมดพร้อมกัน:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**หมายเหตุ** การเปลี่ยนแปลงการตั้งค่านี้อาจใช้เวลาถึงหนึ่งชั่วโมงเพื่อให้มีผล