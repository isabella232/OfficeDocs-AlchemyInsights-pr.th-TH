---
title: ส่งเป็นกลุ่ม Microsoft ๓๖๕
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
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740170"
---
# <a name="send-as-microsoft-365-group"></a>ส่งเป็นกลุ่ม Microsoft ๓๖๕

คุณสามารถกำหนดสิทธิ์ส่งเป็นเพื่ออนุญาตให้ผู้ใช้ที่เฉพาะเจาะจงส่งข้อความเป็นกลุ่ม Microsoft ๓๖๕ดังนี้  

1. เชื่อมต่อกับ Exchange Online PowerShell  

2. เรียกใช้คำสั่งต่อไปนี้:  

    Add-RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs

สำหรับข้อมูลเพิ่มเติมให้ดูที่[อนุญาตให้สมาชิกส่งเป็นหรือส่งในนามของกลุ่ม](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)