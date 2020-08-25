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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="92603-102">ผู้ส่งไม่ได้รับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="92603-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="92603-103">ตามค่าเริ่มต้นผู้ส่งของข้อความอีเมลไปยังกลุ่ม Microsoft ๓๖๕ไม่ได้รับสำเนาของข้อความในกล่องจดหมายเข้าของพวกเขาแม้ว่าผู้ส่งจะเป็นสมาชิกของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="92603-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="92603-104">ใช้คำสั่ง EXO PowerShell นี้เพื่ออนุญาตให้ผู้ส่งได้รับสำเนาของอีเมลแต่ละรายการที่พวกเขาส่งไปยังกลุ่ม Microsoft ๓๖๕ดังนี้</span><span class="sxs-lookup"><span data-stu-id="92603-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="92603-105">เมื่อต้องการเปิดใช้งานการตั้งค่าสำหรับกล่องจดหมายทั้งหมดในครั้งเดียวให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="92603-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="92603-106">**หมายเหตุ:** การเปลี่ยนแปลงการตั้งค่านี้ใช้เวลาถึงหนึ่งชั่วโมงจึงจะมีผล</span><span class="sxs-lookup"><span data-stu-id="92603-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>