---
title: ข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อกโดย SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783822"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="87ad9-102">ข้อผิดพลาดในการส่งอีเมล: โฮสต์ไคลเอ็นต์ถูกบล็อกโดยใช้ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="87ad9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="87ad9-103">ที่อยู่ IP ที่ส่งข้อความอยู่ในรายการบล็อกที่เป็นของ[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="87ad9-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="87ad9-104">เหตุผลสำหรับการบล็อกโดย Spamhaus รวมถึงบัญชีผู้ใช้ที่ถูกบุกรุกเครื่องจักรที่ถูกบุกรุกที่อยู่ IP สาธารณะและนโยบายผู้ให้บริการอินเทอร์เน็ต (ISP)</span><span class="sxs-lookup"><span data-stu-id="87ad9-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="87ad9-105">การแก้ไขที่เป็นไปได้มีดังนี้</span><span class="sxs-lookup"><span data-stu-id="87ad9-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="87ad9-106">สำหรับการบล็อกข้อความขาเข้าที่คุณควบคุมเซิร์ฟเวอร์อีเมลของแหล่งที่มาคุณจำเป็นต้องระบุสาเหตุและเอาบล็อกออกจากเว็บไซต์ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="87ad9-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="87ad9-107">สำหรับการบล็อกข้อความขาเข้าที่ที่อยู่ IP ของแหล่งที่มาเป็นของบุคคลอื่นเจ้าของที่อยู่จะต้องเอาการบล็อกออกจากเว็บไซต์ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="87ad9-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="87ad9-108">ถ้าที่อยู่ IP อยู่บนรายการบล็อกนโยบาย (PBL) เจ้าของสามารถกำหนดที่อยู่ IP แบบคงที่ที่แตกต่างกันหรือเอาที่อยู่ออกจาก PBL</span><span class="sxs-lookup"><span data-stu-id="87ad9-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="87ad9-109">สำหรับข้อความขาออกที่ถูกบล็อกจากโดเมนของคุณที่เชื่อมต่อกับ Microsoft คุณสามารถได้รับข้อผิดพลาดนี้ถ้าข้อความถูกกำหนดเส้นทางผ่านบริการของบริษัทอื่น</span><span class="sxs-lookup"><span data-stu-id="87ad9-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="87ad9-110">คุณสามารถใช้เครื่องมือการค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="87ad9-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
