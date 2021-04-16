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
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813887"
---
# <a name="encryption-with-transport-rules"></a>การเข้ารหัสลับด้วยกฎการส่งผ่าน

ใน [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) คุณสามารถใช้ความสามารถของ Office Message Encryption(OME) ในกฎลําออกจดหมายเพื่อทริกเกอร์การเข้ารหัสลับข้อความได้ เลือกตัวเลือก ใช้ **การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ Office 365** บนเงื่อนไขกฎการส่งผ่าน

- For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- ใน Powershell ให้ใช้ [cmdlet New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) และตั้งค่าพารามิเตอร์ *ApplyOME* $true
