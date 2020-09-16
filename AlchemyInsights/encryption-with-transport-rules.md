---
title: การเข้ารหัสลับที่มีกฎการขนส่ง
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784362"
---
# <a name="encryption-with-transport-rules"></a>การเข้ารหัสลับที่มีกฎการขนส่ง

ใน [ศูนย์การจัดการ Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) คุณสามารถใช้ความสามารถในการเข้ารหัสลับข้อความของ OFFICE (OME) ในกฎโฟลว์จดหมายของคุณเพื่อทริกเกอร์การเข้ารหัสลับข้อความ เลือกตัวเลือกการ **ใช้การเข้ารหัสลับข้อความของ Office ๓๖๕และการป้องกันสิทธิ์** บนเงื่อนไขของกฎการขนส่ง

- สำหรับข้อมูลเพิ่มเติมให้ดู[ที่กำหนดกฎโฟลว์จดหมายเพื่อเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

- ใน Powershell ให้ใช้ cmdlet [TransportRule ใหม่](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) และตั้งค่าพารามิเตอร์ *ApplyOME* เป็น $true
