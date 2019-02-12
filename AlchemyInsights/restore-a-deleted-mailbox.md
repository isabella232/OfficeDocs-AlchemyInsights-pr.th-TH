---
title: การคืนค่ากล่องจดหมายถูกลบไปแล้ว
ms.author: dmaguire
author: msdmaguire
manager: serdars
ms.date: 2/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7b5b4e06-6943-4b2f-b8e4-cdaf13e65c77
ms.openlocfilehash: 9d6a232821884644db08160f18e1dfae2349c349
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29911539"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="f0123-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="f0123-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="f0123-p101">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน ในระหว่างรอบระยะเวลา 30 วันนั้น กล่องจดหมายสามารถถูกกู้คืน โดยการกำหนดสิทธิ์การใช้งานให้กับผู้ใช้อีกครั้ง อย่างไรก็ตาม นี้ได้เท่ากับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="f0123-p101">When a user loses their Exchange Online license, their mailbox is retained for 30 days. During that 30-day period, the mailbox can be recovered by re-assigning the license to the user. However, this is only possible for 30 days.</span></span>
  
<span data-ttu-id="f0123-106">ในเว็บไซต์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="f0123-106">In the Admin Portal:</span></span>
  
- <span data-ttu-id="f0123-p102">ไปยัง**ผู้ใช้** \> **ผู้ใช้ที่ใช้งานอยู่** เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="f0123-p102">Go to **Users** \> **Active users**. Select the user in question.</span></span>
    
- <span data-ttu-id="f0123-109">เลือก \*\* แก้ไข \*\* จะปรับเปลี่ยนสิทธิ์การใช้งานผลิตภัณฑ์</span><span class="sxs-lookup"><span data-stu-id="f0123-109">Select \*\* Edit \*\* to modify product licenses.</span></span> 
    
- <span data-ttu-id="f0123-110">กำหนดสิทธิ์การใช้งานที่ออนไลน์ของ Exchange ไปยังผู้ใช้ จากนั้น**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="f0123-110">Assign the Exchange Online license to the user, and then select **Save**.</span></span>
    
<span data-ttu-id="f0123-p103">กล่องจดหมายที่ใช้ร่วมกันจะได้รับคืนภายใน 30 วัน คุณสามารถค้นหาจดหมายที่ใช้ร่วมกันภายใต้**ผู้ใช้** \> **ผู้ใช้ที่ถูกลบ**ได้ กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="f0123-p103">Shared mailboxes are also recoverable within 30 days. You can find shared mailboxes under **Users** \> **Deleted users**. Shared mailboxes do not require an Exchange Online license.</span></span>
  

