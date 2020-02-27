---
title: สร้างอีเมลที่จับทั้งหมด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286310"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="210a3-102">สร้างอีเมลที่จับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="210a3-102">Create an email catch all</span></span>

<span data-ttu-id="210a3-103">การใช้งานจริง</span><span class="sxs-lookup"><span data-stu-id="210a3-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="210a3-104">มันจะดีกว่าที่จะให้การตีกลับไปยังผู้ส่งที่แจ้งให้ทราบว่าข้อความของพวกเขาไม่สามารถส่งได้ตามที่ระบุเพื่อให้พวกเขาสามารถดำเนินการ</span><span class="sxs-lookup"><span data-stu-id="210a3-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="210a3-105">นอกจากนี้คุณยังสามารถจำกัดการตรวจสอบกล่องจดหมายไปยังที่อยู่อีเมลที่ถูกต้องเดิมจับเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="210a3-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="210a3-106">กล่องจดหมายใดๆที่จับทั้งหมดจะได้รับการจัดการที่ดีของสแปมและในที่สุดอาจจะเติมถ้าไม่ได้รับการตรวจสอบอย่างใกล้ชิด</span><span class="sxs-lookup"><span data-stu-id="210a3-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="210a3-107">(มีข้อจำกัดในการรับ)</span><span class="sxs-lookup"><span data-stu-id="210a3-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="210a3-108">ถ้าคุณตัดสินใจที่จะดำเนินการให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="210a3-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="210a3-109">สร้างกลุ่มการแจกจ่ายแบบไดนามิก & รวม "ผู้รับทุกชนิด"</span><span class="sxs-lookup"><span data-stu-id="210a3-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="210a3-110">สร้างกล่องจดหมายเฉพาะเพื่อตรวจจับอีเมลเช่น catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="210a3-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="210a3-111">สำหรับโดเมนเฉพาะให้ตั้งค่า DomainType เป็น "InternalRelay"</span><span class="sxs-lookup"><span data-stu-id="210a3-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="210a3-112">ถ้าคุณเอาจับทั้งหมดในภายหลังให้แน่ใจว่าได้ตั้งค่าโดเมนกลับไปเป็นสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="210a3-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="210a3-113">สร้างกฎการขนส่ง Mailflow เป็นดังนี้:</span><span class="sxs-lookup"><span data-stu-id="210a3-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="210a3-114">ถ้าผู้ส่งเป็น "ภายนอกองค์กร"</span><span class="sxs-lookup"><span data-stu-id="210a3-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="210a3-115">เปลี่ยนเส้นทางข้อความไป Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="210a3-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="210a3-116">ยกเว้นถ้าผู้รับเป็นสมาชิกของ allusers@domain.com (กลุ่มการแจกจ่ายประกอบด้วยสมาชิกทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="210a3-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="210a3-117">ตรวจสอบให้แน่ใจว่ามีเพิ่มกล่องจดหมายใหม่ลงในกลุ่มการแจกจ่ายแบบไดนามิก</span><span class="sxs-lookup"><span data-stu-id="210a3-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
