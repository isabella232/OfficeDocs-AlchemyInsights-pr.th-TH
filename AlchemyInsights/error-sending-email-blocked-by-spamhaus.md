---
title: ข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อกโดย SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714277"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="199cd-102">ข้อผิดพลาดในการส่งอีเมล: โฮสต์ไคลเอ็นต์ถูกบล็อกโดยใช้ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="199cd-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="199cd-103">ที่อยู่ IP ที่ส่งข้อความอยู่ในรายชื่อบล็อกที่[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)เป็นเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="199cd-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="199cd-104">เหตุผลในการถูกบล็อกโดย Spamhaus ได้แก่ บัญชีที่ถูกบุกรุก เครื่องที่ถูกบุกรุกที่ใช้ที่อยู่ IP สาธารณะร่วมกัน และนโยบายผู้ให้บริการอินเทอร์เน็ต (ISP)</span><span class="sxs-lookup"><span data-stu-id="199cd-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="199cd-105">การแก้ไขที่เป็นไปได้คือ:</span><span class="sxs-lookup"><span data-stu-id="199cd-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="199cd-106">สําหรับข้อความขาเข้าที่ถูกบล็อกซึ่งคุณควบคุมเซิร์ฟเวอร์อีเมลต้นทาง คุณจําเป็นต้องระบุสาเหตุและลบบล็อกจากเว็บไซต์ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="199cd-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="199cd-107">สําหรับข้อความขาเข้าที่ถูกบล็อกซึ่งที่อยู่ IP ของแหล่งที่มาเป็นของบุคคลอื่นเจ้าของที่อยู่ต้องลบบล็อกจากเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="199cd-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="199cd-108">ถ้าอยู่ IP บนนโยบายบล็อกรายการ (PBL), เจ้าของสามารถกําหนดที่อยู่ IP แบบคงที่อื่น หรือเอาที่อยู่จาก PBL</span><span class="sxs-lookup"><span data-stu-id="199cd-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="199cd-109">สําหรับข้อความขาออกที่ถูกบล็อกจากโดเมนของคุณที่เชื่อมต่อกับ Microsoft คุณสามารถรับข้อผิดพลาดนี้หากข้อความถูกส่งผ่านบริการของบริษัทอื่น</span><span class="sxs-lookup"><span data-stu-id="199cd-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="199cd-110">คุณสามารถใช้เครื่องมือค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="199cd-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
