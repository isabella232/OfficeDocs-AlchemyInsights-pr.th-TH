---
title: สมาชิกทุกคนไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479472"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="b58d3-102">สมาชิกทุกคนไม่ได้รับข้อความที่ส่งไปยังกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b58d3-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="b58d3-103">Make sure that all group members have subscribed to receive the emails.</span><span class="sxs-lookup"><span data-stu-id="b58d3-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="b58d3-104">ดู[ติดตามกลุ่ม ใน Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)</span><span class="sxs-lookup"><span data-stu-id="b58d3-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="b58d3-105">เมื่อต้องการตรวจสอบสถานะข้อความของสมาชิกที่สมัครใช้งานอีเมลกลุ่ม ให้เรียกใช้การสั่งต่อไปนี้บน[EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="b58d3-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="b58d3-106">ใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อกําหนดค่าสมาชิกกลุ่มทั้งหมดเพื่อรับอีเมลที่ส่งไปยังกลุ่ม Microsoft 365 ในกล่องจดหมายเข้าของพวกเขา:</span><span class="sxs-lookup"><span data-stu-id="b58d3-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="b58d3-107">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="b58d3-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`