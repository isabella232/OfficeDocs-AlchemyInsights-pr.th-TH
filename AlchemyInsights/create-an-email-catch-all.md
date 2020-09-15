---
title: สร้างอีเมลที่จับทั้งหมด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713005"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="99f0c-102">สร้างอีเมลที่จับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="99f0c-102">Create an email catch all</span></span>

<span data-ttu-id="99f0c-103">การใช้การตรวจจับทั้งหมดเป็นสิ่งที่ไม่น่าสนใจ</span><span class="sxs-lookup"><span data-stu-id="99f0c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="99f0c-104">มันจะดีกว่าที่จะให้การตีกลับไปยังผู้ส่งที่แจ้งให้ผู้ส่งทราบว่าข้อความของพวกเขาไม่สามารถส่งเป็นข้อความเพื่อให้พวกเขาสามารถดำเนินการได้</span><span class="sxs-lookup"><span data-stu-id="99f0c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="99f0c-105">นอกจากนี้คุณยังสามารถจำกัดกล่องจดหมายที่ถูกตรวจสอบเพื่อให้มีเฉพาะที่อยู่อีเมลที่ถูกต้องเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="99f0c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="99f0c-106">กล่องจดหมายที่จับทั้งหมดจะได้รับการจัดการที่ดีของสแปมและในที่สุดอาจเติมถ้าไม่มีการตรวจสอบอย่างใกล้ชิด</span><span class="sxs-lookup"><span data-stu-id="99f0c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="99f0c-107">(มีข้อจำกัดในการรับ)</span><span class="sxs-lookup"><span data-stu-id="99f0c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="99f0c-108">ถ้าคุณตัดสินใจที่จะดำเนินการให้ทำตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="99f0c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="99f0c-109">สร้างกลุ่มการแจกจ่ายแบบไดนามิก & รวมถึง "ชนิดผู้รับทั้งหมด"</span><span class="sxs-lookup"><span data-stu-id="99f0c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="99f0c-110">สร้างกล่องจดหมายที่เฉพาะเจาะจงเพื่อตรวจจับอีเมลตัวอย่างเช่น catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="99f0c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="99f0c-111">สำหรับโดเมนที่เฉพาะเจาะจงให้ตั้งค่า DomainType เป็น "InternalRelay"</span><span class="sxs-lookup"><span data-stu-id="99f0c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="99f0c-112">ถ้าคุณเอาการจับทั้งหมดออกแล้วให้ตรวจสอบให้แน่ใจว่าได้ตั้งค่าโดเมนกลับเป็นสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="99f0c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="99f0c-113">สร้างกฎการขนส่ง Mailflow ดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="99f0c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="99f0c-114">ถ้าผู้ส่งเป็น "อยู่ภายนอกองค์กร"</span><span class="sxs-lookup"><span data-stu-id="99f0c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="99f0c-115">เปลี่ยนเส้นทางข้อความไปยัง Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="99f0c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="99f0c-116">ยกเว้นถ้าผู้รับเป็นสมาชิกของ allusers@domain.com (กลุ่มการแจกจ่ายที่มีสมาชิกทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="99f0c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="99f0c-117">ตรวจสอบให้แน่ใจว่าได้เพิ่มกล่องจดหมายใหม่ลงในกลุ่มการแจกจ่ายแบบไดนามิก</span><span class="sxs-lookup"><span data-stu-id="99f0c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
