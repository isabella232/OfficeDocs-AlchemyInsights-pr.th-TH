---
title: 'เมื่อต้องการกําหนดค่าการตอบกลับอัตโนมัติให้กับอีเมลทั้งหมดที่ส่งไปยังกลุ่ม Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482888"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>เมื่อต้องการกําหนดค่าการตอบกลับอัตโนมัติให้กับอีเมลทั้งหมดที่ส่งไปยังกลุ่ม Microsoft 365:

**เชื่อมต่อกับ EXO PowerShell โดยใช้บัญชีผู้ดูแลระบบผู้เช่า และใช้สั่งต่อไปนี้**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> เปลี่ยน **groupmailbox** เป็นชื่อกลุ่มที่คุณต้องการกําหนดค่าการตอบกลับอัตโนมัติ

