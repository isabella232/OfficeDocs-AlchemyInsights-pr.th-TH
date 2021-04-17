---
title: สร้างอีเมลที่ติดตามทั้งหมด
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816219"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="4388c-102">สร้างอีเมลที่ติดตามทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="4388c-102">Create an email catch all</span></span>

<span data-ttu-id="4388c-103">การใช้สิ่งที่จับได้ทั้งหมดนั้นถูกกีดกันอย่างรัดกุม</span><span class="sxs-lookup"><span data-stu-id="4388c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="4388c-104">คุณควรแจ้งการตีกลับกลับไปยังผู้ส่งเพื่อแจ้งให้ผู้ส่งทราบว่าไม่สามารถส่งข้อความได้ตามที่อยู่เพื่อให้พวกเขาสามารถจัดการได้</span><span class="sxs-lookup"><span data-stu-id="4388c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="4388c-105">คุณยังสามารถจํากัดกล่องจดหมายที่มีการตรวจสอบให้ติดตามเฉพาะที่อยู่อีเมลที่ถูกต้องเดิมเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="4388c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="4388c-106">กล่องจดหมายที่จับได้ทั้งหมดจะได้รับสแปมที่ใช่และอาจเต็มในที่สุดถ้าไม่ได้รับการตรวจสอบอย่างใกล้ชิด</span><span class="sxs-lookup"><span data-stu-id="4388c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="4388c-107">(มีการจํากัดการรับ)</span><span class="sxs-lookup"><span data-stu-id="4388c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="4388c-108">ถ้าคุณตัดสินใจที่จะดําเนินการต่อ ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="4388c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="4388c-109">สร้างกลุ่มการแจกจ่ายแบบไดนามิก&รวมถึง "ชนิดผู้รับทั้งหมด"</span><span class="sxs-lookup"><span data-stu-id="4388c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="4388c-110">สร้างกล่องจดหมายเฉพาะเพื่อติดตามอีเมล ตัวอย่างเช่น catchall@domain.com อีเมล</span><span class="sxs-lookup"><span data-stu-id="4388c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="4388c-111">For the specific domain, set the DomainType to "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="4388c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="4388c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span><span class="sxs-lookup"><span data-stu-id="4388c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="4388c-113">สร้างกฎการส่งผ่านของจดหมายดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4388c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="4388c-114">ถ้าผู้ส่งคือ "ภายนอกองค์กร"</span><span class="sxs-lookup"><span data-stu-id="4388c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="4388c-115">เปลี่ยนเส้นทางข้อความไปยัง Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="4388c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="4388c-116">ยกเว้นถ้าผู้รับเป็นสมาชิกของกลุ่ม allusers@domain.com (กลุ่มการแจกจ่ายมีสมาชิกทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="4388c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="4388c-117">ตรวจสอบให้แน่ใจว่ากล่องจดหมายใหม่ถูกเพิ่มลงในกลุ่มการแจกจ่ายแบบไดนามิก</span><span class="sxs-lookup"><span data-stu-id="4388c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
