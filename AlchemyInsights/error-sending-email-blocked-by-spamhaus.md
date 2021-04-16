---
title: เกิดข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อกโดย SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813743"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c4d86-102">ข้อผิดพลาดในการส่งอีเมล: โฮสต์ไคลเอ็นต์ถูกบล็อกโดยใช้ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="c4d86-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c4d86-103">ที่อยู่ IP ที่ส่งข้อความอยู่ในรายการบล็อกที่เป็นของ[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="c4d86-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="c4d86-104">เหตุผลที่ถูกบล็อกโดย Spamhaus รวมถึงบัญชีที่ถูกละเมิด การใช้งานเครื่องที่ถูกละเมิดการแชร์ที่อยู่ IP สาธารณะ และนโยบายของผู้ให้บริการอินเทอร์เน็ต (ISP)</span><span class="sxs-lookup"><span data-stu-id="c4d86-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="c4d86-105">การแก้ไขที่เป็นไปได้คือ:</span><span class="sxs-lookup"><span data-stu-id="c4d86-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="c4d86-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span><span class="sxs-lookup"><span data-stu-id="c4d86-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="c4d86-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span><span class="sxs-lookup"><span data-stu-id="c4d86-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="c4d86-108">ถ้าที่อยู่ IP อยู่ในรายการบล็อกนโยบาย (PBL) เจ้าของสามารถกําหนดที่อยู่ IP แบบคงที่อื่น หรือเอาที่อยู่ออกจาก PBL ได้</span><span class="sxs-lookup"><span data-stu-id="c4d86-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="c4d86-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span><span class="sxs-lookup"><span data-stu-id="c4d86-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="c4d86-110">คุณสามารถใช้เครื่องมือการค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="c4d86-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
