---
title: กลุ่ม ส่งMicrosoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086147"
---
# <a name="send-as-microsoft-365-group"></a>กลุ่ม ส่งMicrosoft 365

คุณสามารถกําหนดสิทธิ์ ส่งเป็น เพื่ออนุญาตให้ผู้ใช้ที่ระบุส่งข้อความเป็นกลุ่มMicrosoft 365ดังนี้  

1. เชื่อมต่อ Exchange Online PowerShell  

2. เรียกใช้คำสั่งต่อไปนี้:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).