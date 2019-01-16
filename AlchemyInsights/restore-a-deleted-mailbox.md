---
title: การคืนค่ากล่องจดหมายถูกลบไปแล้ว
ms.author: dmaguire
author: msdmaguire
manager: serdars
ms.date: 2/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7b5b4e06-6943-4b2f-b8e4-cdaf13e65c77
ms.openlocfilehash: fc27604014531cc056f853030cf446743a95b36d
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316498"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="fac55-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="fac55-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="fac55-p101">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน ในระหว่างรอบระยะเวลา 30 วันนั้น กล่องจดหมายสามารถถูกกู้คืน โดยการกำหนดสิทธิ์การใช้งานให้กับผู้ใช้อีกครั้ง อย่างไรก็ตาม นี้ได้เท่ากับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="fac55-p101">When a user loses their Exchange Online license, their mailbox is retained for 30 days. During that 30-day period, the mailbox can be recovered by re-assigning the license to the user. However, this is only possible for 30 days.</span></span>
  
<span data-ttu-id="fac55-106">ในเว็บไซต์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="fac55-106">In the Admin Portal:</span></span>
  
- <span data-ttu-id="fac55-p102">ไปยัง**ผู้ใช้** \> **ผู้ใช้ที่ใช้งานอยู่** เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="fac55-p102">Go to **Users** \> **Active users**. Select the user in question.</span></span>
    
- <span data-ttu-id="fac55-109">เลือก \*\* แก้ไข \*\* จะปรับเปลี่ยนสิทธิ์การใช้งานผลิตภัณฑ์</span><span class="sxs-lookup"><span data-stu-id="fac55-109">Select \*\* Edit \*\* to modify product licenses.</span></span> 
    
- <span data-ttu-id="fac55-110">กำหนดสิทธิ์การใช้งานที่ออนไลน์ของ Exchange ไปยังผู้ใช้ จากนั้น**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="fac55-110">Assign the Exchange Online license to the user, and then select **Save**.</span></span>
    
<span data-ttu-id="fac55-p103">กล่องจดหมายที่ใช้ร่วมกันจะได้รับคืนภายใน 30 วัน คุณสามารถค้นหาจดหมายที่ใช้ร่วมกันภายใต้**ผู้ใช้** \> **ผู้ใช้ที่ถูกลบ**ได้ กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="fac55-p103">Shared mailboxes are also recoverable within 30 days. You can find shared mailboxes under **Users** \> **Deleted users**. Shared mailboxes do not require an Exchange Online license.</span></span>
  

