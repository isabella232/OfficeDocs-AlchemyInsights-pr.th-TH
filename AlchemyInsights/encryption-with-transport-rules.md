---
title: การเข้ารหัสลับที่มีกฎการขนส่ง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915286"
---
# <a name="encryption-with-transport-rules"></a>การเข้ารหัสลับที่มีกฎการขนส่ง

ใน[ศูนย์ดูแล Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), คุณสามารถใช้ความสามารถ Office ข้อความการเข้ารหัสลับ (OME) ในกฎการไหลของจดหมายของคุณเพื่อทริกเกอร์การเข้ารหัสลับข้อความ เลือกตัวเลือก**ใช้การเข้ารหัสลับข้อความ Office 365 และการป้องกันสิทธิ์**ในเงื่อนไขกฎการขนส่ง

- สําหรับข้อมูลเพิ่มเติม ให้ดูที่[กําหนดกฎของกระแสจดหมายเพื่อเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

- ใน Powershell ใช้ cmdlet[กฎ TransportRule ใหม่](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities)และตั้งค่าพารามิเตอร์*ApplyOME*เพื่อ$true
