---
title: พูลรีเลย์ขาออก
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381865"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="75e3c-102">พูลรีเลย์ขาออก</span><span class="sxs-lookup"><span data-stu-id="75e3c-102">Outbound relay pool</span></span>

<span data-ttu-id="75e3c-103">Microsoft จะเปลี่ยนแปลงการกําหนดค่าบางอย่างเพื่อรีเลย์หรือส่งต่ออีเมลผ่านMicrosoft 365</span><span class="sxs-lookup"><span data-stu-id="75e3c-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="75e3c-104">ข้อความในบางสถานการณ์จะถูกส่งต่อหรือถ่ายทอดผ่านMicrosoft 365โดยใช้พูลรีเลย์พิเศษ</span><span class="sxs-lookup"><span data-stu-id="75e3c-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="75e3c-105">ข้อความที่ส่งโดยใช้พูลรีเลย์อาจไปอยู่ในโฟลเดอร์อีเมลขยะของผู้รับ</span><span class="sxs-lookup"><span data-stu-id="75e3c-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="75e3c-106">For more information, see [Outbound deliveryพูล](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="75e3c-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="75e3c-107">เมื่อต้องการหลีกเลี่ยงสถานการณ์โดยใช้พูลรีเลย์ ตรวจสอบให้แน่ใจว่าข้อความที่ส่งต่อ/รีเลย์ตรงกับหนึ่งในเกณฑ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="75e3c-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="75e3c-108">ผู้ส่งขาออกเป็นโดเมนที่ยอมรับของผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="75e3c-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="75e3c-109">เฟรมเวิร์กนโยบายตรวจสอบผู้ส่ง (Sender Policy Framework - SPF) จะส่งต่อเมื่อข้อความMicrosoft 365เกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="75e3c-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="75e3c-110">DomainKeys ที่ระบุจดหมาย (DKIM) บนโดเมนผู้ส่ง P2 จะส่งต่อเมื่อข้อความMicrosoft 365ส่ง</span><span class="sxs-lookup"><span data-stu-id="75e3c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="75e3c-111">ข้อความที่ตรงกับเกณฑ์ด้านบนจะไม่ถูกถ่ายทอดผ่านพูลรีเลย์</span><span class="sxs-lookup"><span data-stu-id="75e3c-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="75e3c-112">ถ้าระเบียน MX ของโดเมนของคุณชี้ไปยังเซิร์ฟเวอร์ของบริษัทอื่นหรือเซิร์ฟเวอร์ภายในองค์กร ให้ใช้การกรองขั้นสูงเพื่อให้แน่ใจว่าการตรวจสอบ SPF ถูกต้องกับอีเมลขาเข้าและหลีกเลี่ยงการส่งอีเมลผ่านพูลรีเลย์</span><span class="sxs-lookup"><span data-stu-id="75e3c-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="75e3c-113">**เราจะรู้ได้อย่างไรว่าเราได้รับผลกระทบจากพูลรีเลย์หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="75e3c-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="75e3c-114">ถ้าอีเมลที่ส่งต่อหรือรีเลย์ของคุณใช้หนึ่งในเกณฑ์ข้างต้น ข้อความจะไม่ถ่ายทอดผ่านพูลรีเลย์</span><span class="sxs-lookup"><span data-stu-id="75e3c-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="75e3c-115">อย่างไรก็ตาม ถ้าข้อความถูกส่งผ่านพูลรีเลย์ IP เซิร์ฟเวอร์ขาออกจะอยู่ในช่วง 40.95.0.0/16 และชื่อเซิร์ฟเวอร์ขาออกจะรวม **rly** ในชื่อ</span><span class="sxs-lookup"><span data-stu-id="75e3c-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

