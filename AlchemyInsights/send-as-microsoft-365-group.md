---
title: ส่งเป็นกลุ่ม Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872240"
---
# <a name="send-as-microsoft-365-group"></a>ส่งเป็นกลุ่ม Microsoft ๓๖๕

คุณสามารถกำหนดสิทธิ์ส่งเป็นเพื่ออนุญาตให้ผู้ใช้ที่เฉพาะเจาะจงส่งข้อความเป็นกลุ่ม Microsoft ๓๖๕ดังนี้  

1. เชื่อมต่อกับ Exchange Online PowerShell  

2. เรียกใช้คำสั่งต่อไปนี้:  

    Add-RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs

สำหรับข้อมูลเพิ่มเติมให้ดูที่[อนุญาตให้สมาชิกส่งเป็นหรือส่งในนามของกลุ่ม](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)