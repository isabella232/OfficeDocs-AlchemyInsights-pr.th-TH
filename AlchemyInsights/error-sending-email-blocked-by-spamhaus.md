---
title: ข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อก โดย SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493253"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="9a5d9-102">ข้อผิดพลาดในการส่งอีเมล: โฮสต์ของไคลเอนต์ที่ถูกบล็อคโดยใช้ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="9a5d9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="9a5d9-p101">อยู่ IP ที่ส่งข้อความในรายการบล็อก[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)เป็นเจ้าของอยู่ สาเหตุถูกบล็อคโดย Spamhaus รวมบัญชีถูกโจมตี โจมตีเครื่องที่ใช้ที่อยู่ IP สาธารณะ และนโยบายของผู้ให้บริการอินเทอร์เน็ต (ISP) ร่วมกัน การแก้ไขปัญหาที่เป็นไปได้คือ:</span><span class="sxs-lookup"><span data-stu-id="9a5d9-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="9a5d9-106">หาถูกบล็อคขาเข้าถึง Office 365 ซึ่งคุณควบคุมเซิร์ฟเวอร์อีเมลแหล่งที่มา คุณจำเป็นต้องค้นหาสาเหตุ และบล็อคการเอาออกจากเว็บไซต์ Spamhaus</span><span class="sxs-lookup"><span data-stu-id="9a5d9-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="9a5d9-p102">หาถูกบล็อคขาเข้าไปที่ที่อยู่ IP ของแหล่งที่มาเป็นสมาชิกคนอื่นของ Office 365 เจ้าของที่อยู่ต้องเอาบล็อคจากเว็บไซต์ Spamhaus ถ้าอยู่ IP บนรายการบล็อกนโยบาย (PBL), เจ้าของสามารถกำหนดที่อยู่ IP แบบคงอื่น หรือเอาอยู่จาก PBL</span><span class="sxs-lookup"><span data-stu-id="9a5d9-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="9a5d9-p103">หาถูกบล็อคขาออกจากโดเมน Office 365 ของคุณ คุณสามารถได้รับข้อผิดพลาดนี้ถ้าข้อความถูกจัดเส้นทางผ่านฝ่ายบริการที่ 3 คุณสามารถใช้เครื่องมือค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อค</span><span class="sxs-lookup"><span data-stu-id="9a5d9-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

