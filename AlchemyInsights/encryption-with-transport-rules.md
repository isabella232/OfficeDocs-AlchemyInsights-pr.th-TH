---
title: การเข้ารหัสลับด้วยกฎการส่งผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079469"
---
# <a name="encryption-with-transport-rules"></a>การเข้ารหัสลับด้วยกฎการส่งผ่าน

ใน[ศูนย์Exchangeการจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822)จดหมาย (EAC) คุณสามารถใช้ความสามารถของ Office Message Encryption(OME) ในกฎการโฟลว์จดหมายของคุณเพื่อให้การเข้ารหัสลับข้อความทริกเกอร์ได้ เลือกตัวเลือก การ **การเข้ารหัสลับข้อความของ Office 365และการป้องกัน** สิทธิ์ บนเงื่อนไขกฎการส่งผ่าน

- For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- ใน Powershell ให้ใช้ [cmdlet New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) และตั้งค่าพารามิเตอร์ *ApplyOME* $true
