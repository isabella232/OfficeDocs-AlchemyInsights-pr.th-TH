---
title: ผู้ส่งไม่ได้รับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872238"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>ผู้ส่งไม่ได้รับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕

ตามค่าเริ่มต้นผู้ส่งของข้อความอีเมลไปยังกลุ่ม Microsoft ๓๖๕ไม่ได้รับสำเนาของข้อความในกล่องจดหมายเข้าของพวกเขาแม้ว่าผู้ส่งจะเป็นสมาชิกของกลุ่ม

ใช้คำสั่ง EXO PowerShell นี้เพื่ออนุญาตให้ผู้ส่งได้รับสำเนาของอีเมลแต่ละรายการที่พวกเขาส่งไปยังกลุ่ม Microsoft ๓๖๕ดังนี้  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

เมื่อต้องการเปิดใช้งานการตั้งค่าสำหรับกล่องจดหมายทั้งหมดในครั้งเดียวให้ทำดังนี้

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**หมายเหตุ:** การเปลี่ยนแปลงการตั้งค่านี้ใช้เวลาถึงหนึ่งชั่วโมงจึงจะมีผล