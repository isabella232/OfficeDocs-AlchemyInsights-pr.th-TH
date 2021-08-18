---
title: 'เมื่อต้องการกําหนดค่าการตอบกลับอัตโนมัติให้กับอีเมลทั้งหมดที่ส่งMicrosoft 365ให้:'
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
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331550"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>เมื่อต้องการกําหนดค่าการตอบกลับอัตโนมัติให้กับอีเมลทั้งหมดที่ส่งMicrosoft 365ให้:

**เชื่อมต่อ EXO PowerShell โดยใช้บัญชีผู้ดูแลระบบผู้เช่า และใช้การสั่งต่อไปนี้**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**หมายเหตุ**: **เปลี่ยน groupmailbox** เป็นชื่อกลุ่มที่คุณต้องการกําหนดค่าการตอบกลับอัตโนมัติ

