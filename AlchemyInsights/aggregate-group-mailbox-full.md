---
title: AggregateGroupMailbox ทั้งหมด NDR ที่ได้รับสำหรับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722077"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox ทั้งหมด NDR ที่ได้รับสำหรับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕

ใช้คำสั่งต่อไปนี้ของ EXO Shell เพื่อสร้างกฎการขนส่ง Exchange เพื่อลดอีเมลที่ส่งไปยังกล่องจดหมายรวมของกลุ่มดังนี้

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> แทนที่อยู่ SMTP ใน **SentTo** ที่มีที่อยู่ smtp ของกล่องจดหมายการรวมกลุ่มในผู้เช่าของคุณ คุณสามารถรับที่อยู่ SMTP ของกล่องจดหมายกลุ่มการรวมจาก NDR ที่ได้รับ



