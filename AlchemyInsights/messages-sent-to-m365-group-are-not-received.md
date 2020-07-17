---
title: สมาชิกทั้งหมดไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051519"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="a9b26-102">สมาชิกทั้งหมดไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a9b26-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="a9b26-103">ตรวจสอบให้แน่ใจว่าสมาชิกกลุ่มทั้งหมดได้สมัครรับอีเมล</span><span class="sxs-lookup"><span data-stu-id="a9b26-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="a9b26-104">ดู[ติดตามกลุ่มใน Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)</span><span class="sxs-lookup"><span data-stu-id="a9b26-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="a9b26-105">เมื่อต้องการตรวจสอบสถานะข้อความของสมาชิกที่สมัครเป็นสมาชิกอีเมลกลุ่ม ให้เรียกใช้คําสั่งต่อไปนี้บน[EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="a9b26-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`