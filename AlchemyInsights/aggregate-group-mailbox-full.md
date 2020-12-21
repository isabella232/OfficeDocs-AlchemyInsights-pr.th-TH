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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="6e513-102">AggregateGroupMailbox ทั้งหมด NDR ที่ได้รับสำหรับอีเมลที่ส่งไปยังกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="6e513-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="6e513-103">ใช้คำสั่งต่อไปนี้ของ EXO Shell เพื่อสร้างกฎการขนส่ง Exchange เพื่อลดอีเมลที่ส่งไปยังกล่องจดหมายรวมของกลุ่มดังนี้</span><span class="sxs-lookup"><span data-stu-id="6e513-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="6e513-104">แทนที่อยู่ SMTP ใน **SentTo** ที่มีที่อยู่ smtp ของกล่องจดหมายการรวมกลุ่มในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="6e513-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="6e513-105">คุณสามารถรับที่อยู่ SMTP ของกล่องจดหมายกลุ่มการรวมจาก NDR ที่ได้รับ</span><span class="sxs-lookup"><span data-stu-id="6e513-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



