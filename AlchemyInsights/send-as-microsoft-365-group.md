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
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="af0d0-102">ส่งเป็นกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="af0d0-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="af0d0-103">คุณสามารถกำหนดสิทธิ์ส่งเป็นเพื่ออนุญาตให้ผู้ใช้ที่เฉพาะเจาะจงส่งข้อความเป็นกลุ่ม Microsoft ๓๖๕ดังนี้</span><span class="sxs-lookup"><span data-stu-id="af0d0-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="af0d0-104">เชื่อมต่อกับ Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="af0d0-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="af0d0-105">เรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="af0d0-105">Run the following command:</span></span>  

    <span data-ttu-id="af0d0-106">Add-RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="af0d0-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="af0d0-107">สำหรับข้อมูลเพิ่มเติมให้ดูที่[อนุญาตให้สมาชิกส่งเป็นหรือส่งในนามของกลุ่ม](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="af0d0-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>