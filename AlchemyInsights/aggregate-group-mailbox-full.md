---
title: AggregateGroupMailbox ได้รับ NDR แบบเต็มเพื่อให้อีเมลที่Microsoft 365กลุ่ม
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951872"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox ได้รับ NDR แบบเต็มเพื่อให้อีเมลที่Microsoft 365กลุ่ม

ใช้สั่ง EXO Shell ต่อไปนี้เพื่อสร้างกฎการส่งผ่านExchangeไปยังอีเมลที่ปล่อยโดยไม่แสดงการแจ้งเตือนที่ส่งไปยังกล่องจดหมายของกลุ่มรวม:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> แทนที่ที่อยู่ SMTP ใน **-SentTo ด้วย** ที่อยู่ SMTP ของกล่องจดหมายของกลุ่มการรวมในผู้เช่าของคุณ คุณสามารถรับที่อยู่ SMTP ของกล่องจดหมายของกลุ่มการรวมจาก NDR ที่ได้รับ



