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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315929"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox ได้รับ NDR แบบเต็มเพื่อให้อีเมลที่Microsoft 365กลุ่ม

ใช้สั่ง SHELL ของ EXO ต่อไปนี้เพื่อสร้างกฎExchangeส่งไปยังอีเมลที่ปล่อยโดยไม่แสดงการแจ้งเตือนที่ส่งไปยังกล่องจดหมายของกลุ่มรวม:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**หมายเหตุ**: แทนที่ที่อยู่ SMTP ใน **-SentTo** ด้วยที่อยู่ SMTP ของกล่องจดหมายกลุ่มการรวมในผู้เช่าของคุณ คุณสามารถรับที่อยู่ SMTP ของกล่องจดหมายของกลุ่มการรวมจาก NDR ที่ได้รับ



